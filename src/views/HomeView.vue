<template>
    <h1>Welcome</h1>
    <h2>Silahkan Login Terlebih Dahulu</h2>

    <div class="row justify-content-md-center">
    <div class="col-md-3">
      <div>
        <div class="card-header">Login</div>
        <div class="card-body"></div>
        <form>
          <div class="form-group">
            <label for="NIM">NIM</label>
            <input type="text" required class="form-control" placeholder=""/>
          </div>

          <div class="form-group">
            <label for="Nama">Nama</label>
            <input type="text" required class="form-control" placeholder=""/>
          </div>
          <button type="submit" class="btn btn-primary">Login</button>
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
