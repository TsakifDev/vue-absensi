<template>
<div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-6">
                    <div class="card mt-5">
                        <div class="card-body">
                            <h3 class="text-center">Absensi Kehadiran</h3>
                             <!-- form validasi -->
                            <form @submit.prevent="handleSubmit">
                              <div class="form-group mt-2">
                                    <label>Nama</label>
                                    <input class="form-control" placeholder="Nama lengkap anda" type="name" v-model="nama" required>
                              </div>
                              <div class="form-group mt-2">
                                    <label for="pekerjaan">Jenis Kelamin</label>
                                    <select class="form-control" v-model="gender">
                                        <option value="laki">Laki-Laki</option>
                                        <option value="Perempuan">Perempuan</option>
                                    </select>
                                </div>
                                <div class="form-group mt-2">
                                    <label>Kelas</label>
                                    <select class="form-control" v-model="kelas">
                                        <option value="7">7</option>
                                        <option value="8">8</option>
                                        <option value="9">9</option>
                                        <option value="10">10</option>
                                        <option value="11">11</option>
                                        <option value="12">12</option>
                                    </select>
                                </div>
                                <div class="form-group mt-3 mb-3">
                                    <input class="btn btn-primary" type="submit" value="Submit">
                                </div>
                            </form>
                            <div class="p-3 rounded-2 border border-secondary">
                              <p>Nama : {{nama}}</p>
                              <p>Jenis kelamin : {{gender}}</p>
                              <p>Kelas : {{kelas}}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
  data(){
    return {
      nama: '',
      gender: '',
      kelas: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
