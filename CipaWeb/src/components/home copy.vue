<template>

  <nav class="navbar bg-primary navbar-expand-lg ">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">
        <img src="/public/perfil.png" alt="EcoLogica" width="65" height="55">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Perfil</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#" @click="navigateToHome">Inicio</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Parceiros
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#" style="color:black!important;">Parceiros Cadastrados</a></li>
              <li><a class="dropdown-item" href="#" style="color:black!important;">Futuros Parceiros</a></li>
              <li><hr class="dropdown-divider" style="color:black!important;"></li>
              <li><a class="dropdown-item" href="#" style="color:black!important;">Seja nosso parceiro</a></li>
            </ul>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
  <br>
  <hr>
  <div class="card">
    <div class="information">
  
    <div class="topCard">
      <img src="/public/perfil.png">
    <span>Pedro Henrique</span>
  <br>
    </div>
  <div class="infoCard">
    <section class="box">
    <img src="/public/2(1).png">
    <span>EcoPoints: 30</span>
  </section>
  <section class="box">
    <img src="/public/1(1).png">
    <span>EcoCoins: R$20</span>
  </section>
  <section class="box">
    <img src="/public/3.png">
    <button type="button" class="btn btn-outline-success">EcoTransfer</button>
  </section>
  </div>
  
  </div>
  </div>
  
  <!-- Rodapé do Site -->
  <footer class="bg-light text-center text-white">
    <!-- Grid container -->
    <div class="container p-4 pb-0">
      <!-- Section: Social media -->
      <section class="mb-4">
        <!-- Facebook -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #3b5998;"
          href="#!"
          role="button"
          ><i class="fab fa-facebook-f"></i
        ></a>
  
        <!-- Twitter -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #55acee;"
          href="#!"
          role="button"
          ><i class="fab fa-twitter"></i
        ></a>
  
        <!-- Google -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #dd4b39;"
          href="#!"
          role="button"
          ><i class="fab fa-google"></i
        ></a>
  
        <!-- Instagram -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #ac2bac;"
          href="#!"
          role="button"
          ><i class="fab fa-instagram"></i
        ></a>
  
        <!-- Linkedin -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #0082ca;"
          href="#!"
          role="button"
          ><i class="fab fa-linkedin-in"></i
        ></a>
        <!-- Github -->
        <a
          class="btn text-white btn-floating m-1"
          style="background-color: #333333;"
          href="#!"
          role="button"
          ><i class="fab fa-github"></i
        ></a>
      </section>
      <!-- Section: Social media -->
    </div>
    <!-- Grid container -->
  
    <!-- Copyright -->
    <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
      © 2023 Copyright:
      <a class="text-white" href="https://mdbootstrap.com/">CipaWeb</a>
    </div>
    <!-- Copyright -->
  </footer>
  </template>
  
  <style scoped>
  .carousel-control-next-icon{
    color:black!important;
    background-color: #1E2F40!important;
  }
  .visually-hidden{
    color:red;
  }
  
  .ContentCardMobile{
    display: none;
  }
  .navbar a,p,h1,h2,span{
      color: white!important;
  }
  .cards-groups{
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      height: 100vh;
  }
  .card{
      background-color: #fff;
      border-radius: 20px;
      box-shadow: 0px 2px 23px #26395338;
      min-width: 220px;
      min-height: 270px;
      margin-left: 2%;
  
  }
  .information img{
    width: 120px;
  }
  .mediaCard{
      display: flex;
      align-items: center;
      justify-content: center;
  }
  .information{
    display: flex;
    flex-direction: column;
  }
  .infoCard{
    display: inline-block;
    width: 100%;
  }
  .topCard span{
    font-weight: bold;
    font-size: 26px;
    border: 1px solid black;
    padding-left: 12px;
    padding-right: 12px;
  }
  .d-flex button{
      background-color: green!important;
      color: white!important;
  }
  *{
    color: black!important;
  }
  .mediaCard img{
      width: 220px;
  }
  .topCard{
      padding: 20px;
      padding-top: 0px;
  }
  .information{
    display: flex;
    justify-content: center;
    align-items: center;
  
  }
  .box{
    display: inline-block;
    margin-left: 2%;
      
  }
  .box span{
    color: black!important;
  }
  
  .card span, h2, h1, p{
    color: black!important;
  }
  .card{
    text-align: center;
  }
  .contents{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .vote{
      background-color: #D4BF06;
      border: none;
      padding: 8px 20px 8px 20px;
      border-radius: 5px;
      color: black;
      font-weight: bold;
      margin-right: 7%;
  }
  .report{
      background-color: #ff4800;
      border: none;
      padding: 8px 20px 8px 20px;
      border-radius: 5px;
      color: white;
      font-weight: bold;
  }
  </style>
  
  <script>
  export default {
    methods: {
      navigateToHome() {
        this.$router.push('/home')
      }
    }
  }
  </script>