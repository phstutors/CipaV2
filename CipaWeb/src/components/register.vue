<template>

<div class="app">
  <div class="content">
    <section class="left-side">
      <div class="agroup-content">
        <img src="public/FundoCipa.png" alt="" srcset="">
        <h2>CIPA WEB</h2>
        <p>Concurso de Ideias <br>Professor Anjo</p>
      </div>
    </section>


    <!-- Right side of the page-->
    <div class="right-side">
    <img src="/public/C.png">
    <p>Por favor, insira seus <br/>dados para se cadastrar</p>
    <div id="inputs-group">
        <div class="mb-3 row">
          <div class="col-sm-10">
              <label for="staticEmail">Nome:</label>
              <input type="text" class="form-control" id="staticEmail" placeholder="Steve Jobs">
          </div>
        </div>
        <div class="mb-3 row">
          <div class="col-sm-10">
          <label for="staticPassword">Digite seu Email:</label>
          <input type="password" class="form-control" id="inputPassword" placeholder="YourEmail@gmail.com">
        </div>
      </div>

      <div class="mb-3 row">
          <div class="col-sm-10">
          <label for="staticPassword">Escolha sua Senha:</label>
          <input type="password" class="form-control" id="inputPassword" placeholder="********">
        </div>
      </div>
      <div class="mb-3 row">
      <label for="staticPassword">Escolha sua Senha:</label>
          <select class="form-select" aria-label="Default select example">
            <option selected>Estudante</option>
            <option value="1">Professor</option>
            <option value="2">Instituição</option>
          </select>
    </div>


      <button type="button" class="btn btn-primary btn-lg">Entrar</button>
    </div>
    </div>
  


  </div>
  </div>
</template>

<style scoped>
.app {
  width: 100%;
  height: 100vh;
  margin:0;
  display: flex!important;
  justify-items: center!important;
  justify-content: center!important;
  align-items: center!important;

}
.teste {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #F1F4FF;
  font-family: 'Red Hat Display', sans-serif!important;
}
.right-side p{
font-size: 15pt;
}
h2,p{
color: #1E2F40!important;
}

.content {
  height: 80%;
  width: 80%;
  display: flex;
  box-shadow: 0 8px 10px rgba(0, 0, 0, 0.1);
}

.left-side {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  width: 50%;
  flex-direction: column;
  background-color: antiquewhite;

}

.right-side {
  width: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  justify-items: center;
  flex-direction: column;
  border-left: 0.1rem solid black;
  background-color: antiquewhite;
  
}
.agroup-content img{
  width: 720px;
  animation: pulse 8s ease-in-out infinite;
}
.agroup-content h2{
  font-family: 'Red Hat Display', sans-serif;
  font-size: 50pt;
}
.agroup-content p{
  font-family: 'Red Hat Display', sans-serif;
  font-size: 20pt;
}
.right-side img{
width: 270px;
animation: flutuar 2s ease-in-out infinite;
}

#inputs-group{
width: 100%!important;
display: flex;
flex-direction: column;
justify-content: center;
justify-items: center;
align-items: center;
}
.mb-3{
width: 80%!important;
}
.mb-3 select{
width: 82%!important;
}
button{
background-color: #4AB7AA;
border: none;
color: #fff;
padding-left: 20px!important;
padding-right: 20px!important;
box-shadow: 0 8px 10px rgba(0, 0, 0, 0.1);
}
button:hover{
background-color: #1A314B!important;
animation: pulseAnimation 2s ease-in-out infinite!important;
}

@keyframes pulseAnimation {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
  100% {
    transform: scale(1);
  }
}
@keyframes flutuar {
0% { transform: translateY(0); }
50% { transform: translateY(-20px); }
100% { transform: translateY(0); }
}
@keyframes pulse {
0% { transform: scale(1); }
50% { transform: scale(1.1); }
100% { transform: scale(1); }
}
</style>
