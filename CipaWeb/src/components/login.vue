<template>
  <div class="content">
    
    <div class="left-side">
      <div class="agroup-content">
        <img src="public/FundoCipa.png" alt="" srcset="">
        <h2>CIPA WEB</h2>
        <p>Concurso de Ideias <br>Professor Anjo</p>
      </div>
    </div>
    


    <!-- Right side of the page-->
    <div class="right-side">
      <img src="/public/C.png">
    <p>Por favor, insira seus <br/>dados para se cadastrar</p>
    <div id="inputs-group">
        <div class="mb-3 row">
          <div class="col-sm-10">
              <label for="staticEmail">Digite seu Email:</label>
              <input type="text" class="form-control" id="staticEmail" placeholder="email@example.com" v-bind:class="{ error: !emailValid }" v-model="email" @input="checkEmail">
          </div>
        </div>
        <div class="mb-3 row">
          <div class="col-sm-10">
          <label for="staticPassword">Digite sua Senha:</label>
          <input type="password" class="form-control" id="inputPassword" placeholder="********">
        </div>
        
      </div>
      <button type="button" class="btn btn-primary btn-lg">Entrar</button>
    </div>

  
  </div>
  </div>
</template>

<style scoped>



.right-side p{
font-size: 15pt;
}
h2,p{
color: #1E2F40!important;
}.teste {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #F1F4FF;
  font-family: 'Red Hat Display', sans-serif!important;
}

.content {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 8px 10px rgba(0, 0, 0, 0.1);
  border-radius: 42px;
  background-color: #F1F4FF;
  font-family: 'Red Hat Display', sans-serif!important;
}

.left-side {
  width: 40%;
  height: 70%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: antiquewhite; 
  border-bottom-left-radius: 25px;
 border-top-left-radius: 25px;

}

.right-side {
  width: 40%;
  height: 70%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  justify-items: center;
  border-left: 0.1rem solid black;
  background-color: antiquewhite;
  border-bottom-right-radius: 25px;
 border-top-right-radius: 25px;
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
<script>

export default {
  name: "login",
  data() {
    return {
      email: "",
      senha: "",
      emailValid: true,
    };
  },
  methods: {
     logar() {
    
     
    },
    cadastre() {
      this.$router.push("cadastro");
    },
    recuperar() {
      return this.$router.push("/email");
    },
    checkEmail(){
      if (!this.email.endsWith('discente.ifpe.edu.br')) {
        this.emailIsValid = false;
      } else {
        this.emailIsValid = true;
      }
    }
  },
};
</script>
