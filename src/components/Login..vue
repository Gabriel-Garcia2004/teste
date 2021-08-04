<template>
  <section class="login">
    <div class="login__container">
      
      <img class="login__ninja-lecdt-1" src="../assets/img-1.png" alt="Ilustração">
      <img class="login__ninja-lecdt-2" src="../assets/img-2.png" alt="Ilustração">
      <div class="login__box">
        <hgroup>
          <h2 class="login__subtitle">Teste dos</h2>
          <h1 class="login__title" >Mestres</h1> 
        </hgroup>
        <div class="login__inputs">
        <label class="login__label" for="email">Email de login <span class="login__span">*</span> </label>
         <input class="login__input" id="email" type="email" placeholder="email@email.com">
         <label class="login__label" for="email">Senha de login <span class="login__span">*</span> </label>
         <input class="login__input" id="email" type="password" placeholder="senha123#">
         <a href="#" class="login__button">ENTRAR AGORA <span class="login__button-span">></span></a>
        </div>
            <p class="login__text">Não tem conta? <a href="#" class="login__link">Crie agora.</a> </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'login',
  props: {
    msg: String
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
@font-face {
  font-family: ccmonster;
  src: url("../assets/ccmonster.ttf");
}

.login{
  background-image: url('../assets/fundo-1.png');
  background-repeat: no-repeat;
  

}
.login__container{
  background-image: url('../assets/fundo-2.png');
  background-repeat: no-repeat;
  background-size: 100vw;
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr;
  max-width: 100%;
  height: 100vh;

}
.login__ninja-lecdt-1{
  width: 85%;
  min-width: 200px;
  max-height: 60vh;
  object-fit: cover;
  object-position: center top;
  justify-self: flex-end;
  align-self: flex-end;
  grid-column: 1/2;
  grid-row: 1/2;
  transform: scaleX(-1);

}
.login__ninja-lecdt-2{
  max-width: 50%;
  min-width: 200px;
  max-height: 60vh;
  object-fit: cover;
  object-position: center top;
  justify-self: flex-start;
  grid-column: 1/1;
  grid-row: 1/1;
  transform: scale(-1, -1);

}
.login__box{
  max-width: 550px;
  grid-column: 1/2;
  grid-row: 1;
  justify-self: center;
  align-self: center;
  background: linear-gradient(30deg,#141b2c, #112b5c);
  opacity: .99;
  border-radius: 1rem;
  padding: 30px 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content:  center;
  gap:  50px 0;
  margin: 5px;
  grid-row: 1/2;

}
.login__title{
  font-family: ccmonster;
  text-align: center;
  font-size: 4.75rem;
  color: #fff;
}
.login__subtitle{
  text-align: center;
  font-size: 1.8125rem;
  color: #fff;

}
.login__inputs{
  display: flex;
  flex-direction: column;
  gap: 10px 0;
}
.login__label{
  color: #fff;
font-size: 0.75rem;
padding: 0 0.3125rem;
}
.login__span{
  color: #FF031D;
}
.login__input{
background: #FFFFFF 0% 0% no-repeat padding-box;
border-radius: 0.8125rem;
opacity: 0.06;
padding: 0.625rem;
outline: transparent;
transition: .5s ease;
}
.login__input:hover{
  opacity: 0.1;
}
.login__button{
  font-family: ccmonster;
  font-size: 33px;
  background: #005FFF;
  color: #fff;
  outline: transparent;
  padding: 0.4375rem;
  border: transparent;
  border-radius: 13px;
  text-decoration: none;
  opacity: .8;
}
.login__button:hover{
  opacity: 1;

}
.login__button-span{
  padding-left: 15px ;
}
.login__text{
  color: #fff;
  font-size: 19px;
}
.login__link{
  color: #005FFF;
  text-decoration: none;
  opacity: .8;
}
.login__link:hover{
  opacity: 1;
}
@media (min-width: 1024px) {
  .login__container{
  background-image: url('../assets/fundo-2.png');
  background-repeat: no-repeat;
  background-size: 100vw;
display: grid;
      grid-template-columns: 1fr 1fr 1fr;
  max-width: 100%;
  height: 100vh;


}
  .login__box{
  width: 350px;
  grid-column: 2/2;

    
  }
  .login__ninja-lecdt-1{
    width: unset;
  max-width: 890px;
  min-width: 200px;
  max-height:95vh;
  object-fit: contain;
  justify-self: flex-start;
  align-self: flex-end;
  grid-column: 1/2;
  transform: scaleX(1);

  
}
.login__ninja-lecdt-2{
  max-width: 840px;
  min-width: 200px;
  max-height: 100vh;
  object-fit: contain;
  justify-self: flex-end;
  grid-column: 3/3;
  grid-row: 1;
  align-self: flex-end;
  transform: scaleY(1);

}



}
</style>
