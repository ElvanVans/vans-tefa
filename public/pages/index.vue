<template>
    <div class="container-fluid">
      <div class="statistik">
      <h1>STATISTIK</h1>
      </div>
      <div class="row my-5 d-flex justify-content-evenly ">
        <div class="col-lg-6 box">
          <NuxtLink to="/pengunjung/tambah">
            <div class="card bg-pengunjung rounded-5">
              <div class="card-body">
                <div class="Elvan">
                  <h2>Pengunjung</h2>
                </div>
              </div>
            </div>
          </NuxtLink>
        </div>
        <div class="col-lg-6 box">
          <NuxtLink to="/buku">
            <div class="card bg-buku rounded-5">
              <div class="card-body">
                <div class="Elvan">
                  <h2>Buku</h2>
                </div>
              </div>
            </div>
          </NuxtLink>
        </div>
      </div>
        <div class="row my-5 d-flex justify-content-evenly ">
          <div class="col-lg-6 box">
            <div class="card b2 rounded-5">
              <div class="card-body text">
                <h1 class="no">5</h1>
                <p class="yes">Pengunjung</p>
              </div>
            </div>
          </div>
          <div class="col-lg-6 box">
            <div class="card b3 rounded-5">
              <div class="card-body text">
                <h1 class="no">30</h1>
                <p class="yes">Buku</p>
              </div>
            </div>
          </div>
        </div>
        <div class="container">
          <div class="row">
            <Statistik />
          </div>
        </div>
      </div>
    </template>
  
  <script setup>
  useHead({ title: "Home/Perpustakaan Digital" })
  </script>
  
  <style scoped>
  .card {
    height: 250px;
  }
  .card.bg-pengunjung{
    background-image: url('../assets/img/pengunjung.jpg');
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
    color: black;
  }
  .card.bg-buku {
    background: url('../assets/img/perpustakaan.jpg') no-repeat center center;
    background-size: cover;
    color: black;
  }
  .statistik {
    color: rgba(0, 0, 0, 0.761);
    margin-left: 30px;
  }
  .box{
    width: 45%;
  }
  .box a{
    text-decoration: none;
  }
  .b2{
    background-color: #C869C4;
  }
  .b3{
    background-color: #1F752D;
  }
  .text{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .no{
    font-size: 70px;
  }
  .yes{
    font-family: 'Times New Roman', Times, serif;
    font-size: 25px;
    padding-top: 40px;
  }
  .Radi{
    color: rgb(255, 255, 255);
    font-family: 'Times New Roman', Times, serif;
  }
  </style>