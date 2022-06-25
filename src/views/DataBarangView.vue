<template>
  <div class="container mt-5">
    <h2>Data Barang</h2>
    <button class="btn btn-primary btn-sm float-left">
      <span class="icon is-small">
        <i class="fas fa-plus"></i>
      </span>
      Tambah Barang</button>
  </div>
  <table class="container table table-sm mt-3">
    <thead>
    <tr>
      <th>No.</th>
      <th>Nama Barang</th>
      <th>Gambar</th>
      <th>Kondisi</th>
      <th>Kategori</th>
      <th>Tanggal Update</th>
      <th>Aksi</th>
    </tr>
    </thead>
    <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Laptop macbook m1</td>
      <td>
        <img src="../assets/laptop.png" class="card-img" alt="...">
      </td>
      <td>Tersedia</td>
      <td>Laptop</td>
      <td>22 juni 2022</td>
      <td>
        <button class="btn btn-primary"> Detail </button> |
        <button class="btn btn-success"> Edit </button> |
        <button class="btn btn-danger"> Hapus </button>
      </td>
    </tr>
    </tbody>

    <tbody>
    <tr>
      <th scope="row">2</th>
      <td>Nikon D3300</td>
      <td>
        <img src="../assets/camera.png" class="card-img" alt="...">
      </td>
      <td>Tersedia</td>
      <td>Kamera</td>
      <td>19 juni 2022</td>
      <td>
        <button class="btn btn-primary"> Detail </button> |
        <button class="btn btn-success"> Edit </button> |
        <button class="btn btn-danger"> Hapus </button>
      </td>
    </tr>
    </tbody>

    <tbody>
    <tr>
      <th scope="row">3</th>
      <td>canon pixma mp287</td>
      <td>
        <img src="../assets/proyektor.png" class="card-img" alt="...">
      </td>
      <td>Tersedia</td>
      <td>Proyektor</td>
      <td>16 juni 2022</td>
      <td>
        <button class="btn btn-primary"> Detail </button> |
        <button class="btn btn-success"> Edit </button> |
        <button class="btn btn-danger"> Hapus </button>
      </td>
    </tr>
    </tbody>

  </table>

</template>

<script>

</script>


<Style>
div {
  margin-bottom: 100px;
}
</Style>