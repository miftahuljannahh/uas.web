<template>
    <div class="row justify-content-md-center">
    <div class="col-md-4">
      <div>
        <div class="card-header">Login</div>
        <div class="card-body"></div>
        <form>
          <div class="form-group">
            <label for="NIM">ID</label>
            <input type="text" required class="form-control" placeholder="Masukkan ID" autofocus>
          </div>

          <div class="form-group">
            <label for="Nama">Nama</label>
            <input type="text" required class="form-control" placeholder="Masukkan Nama" autofocus>
          </div>
          <div class="form-group">
            <label for="level">Level</label>
            <select name="level" id="level" class="form-control">
              <option value="">-- Masuk Sebagai --</option>
              <option value="2">User</option>
              <option value="1">Admin</option>
            </select>
          </div>
          <button type="submit" class="btn btn-primary btn-block">Login</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  },
  data() {
    return {
      nim: '',
      nama: ''
    }
  }
}
</script>

<style scoped>
h1{
  padding-top: 30px;
}
h2 {
  padding-bottom: 40px;
}
label{
margin-right: 700px;
color: rgb(38, 15, 27);
}

</style>
