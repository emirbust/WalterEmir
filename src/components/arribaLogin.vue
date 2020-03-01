<template>
    <div class="titulo">
       <section class="hero">
          <div class="hero-body">
                    <img class="tamaño" src="../assets/Logo_Netflix.png" alt="">
          </div>
        </section>
        <div class="container">
            <div class="card">
                  <div class="card-content">
                    <h1 class="title is-3">
                      Inicia Sesion
                      </h1>
                    <h2 class="subtitle is-6">
                      inicia sesion para conmenzar a ver o reiniciar tu membresia.
                      </h2>
                      <div class="field">
                          <p class="control">
                            <input class="input is-medium" type="email">
                          </p>
                          <label for="" class="letras">Email o numero de telefono</label>
                      </div>
                      <div class="field">
                          <p class="control">
                            <input class="input is-medium" type="password">
                          </p>
                          <label for="" class="letras">Email o numero de telefono</label>
                      </div>
                      <div class="buttons">
                        <b-button @click="login" class="button is-medium" type="" expanded><h3 style="color: aliceblue;" class="is-size-5 has-text-centered">iniciar sesion</h3></b-button>
                      </div>
                      <div class="level">
                        <div class="level-left">
                          <div class="level-item">
                           <div class="field">
                            <b-checkbox style="color: rgb(140, 140, 140);" type="is-danger" native-value="Nope">Recuerdame</b-checkbox>
                            </div>
                          </div>
                        </div>
                        <div class="level-right">
                          <div class="level-item">
                            <a class="ayuda" href="">¿Necesitas ayuda?</a>
                          </div>
                        </div>
                    </div>
                    <div class="level">
                      <div class="level-left">
                        <div class="imagefc">
                          <figure class="image is-16x16">
                            <img src="../assets/fb_icon_325x325.png">
                          </figure>
                        </div>
                         <a class="iniciofc" href="">Inicia sesion con Facebook</a>
                      </div>
                    </div>
                    <div style="width: 322px; height: 1px; background-color: rgba(102, 101, 101, 0.9); top: 50%; position: relative; margin: 6%; left: -6%;"></div>
                    <div>
                      <h3 style="font-size: 20px; margin-top: -3.9px; font-weight: bold; color: aliceblue;">¿primera vez en Netflix?</h3>
                      <h4 style="color: aliceblue; top: 30%; ">Sin publicidad.
                        disfruta donde quieras.
                        Cancela en cualquier momento.
                      </h4>
                      <div class="buttons">
                        <b-button id="btonn" class="button is-medium" type="is-light" expanded><h5 class="is-size-5 has-text-centered">Suscribete ahora ></h5></b-button>
                      </div>
                    </div>
                  </div>
            </div>
        </div>
     </div>
</template>

<script>
export default {
  name: 'arribaLogin',
  props: {
    msg: String
  },
  methods: {
    login () {
      this.$router.push('/login')
    }
  }
}
</script>

<style scoped>
.tamaño{
  width: 210px;
  height: 130px;
  position:absolute;
  top: -3%;
  left: 1.2%;
}
.card{
  background-color: rgba(0, 0, 0, 0.8);
  width: 450px;
  height: 700px;
  top: 302px;
  left: 52%;
  transform: translate(-50%, -50%);
}
h1{
  color:aliceblue;
  padding-top: 9.7%;
}
h2{
  color:aliceblue;
  padding-top: 3.5%;
}
.card-content{
  margin: 9%;
}
.letras{
  position:absolute;
  padding-left: 15px;
  margin-top: -34px;
  z-index: -20;
  color: rgb(140, 140, 140);
  transition: 2ms
}
.input{
  background: rgba(102, 101, 101, 0.5);
  border:none;
  margin-top: 5px;
}
.input:focus {
  background:rgba(114, 113, 113, 0.5);
  outline: rgba(140, 140, 140, 0.3)
}
.letras:focus{
  margin-top: 200%;
}
.buttons{
  margin-top: 40px;
  padding-top: -10px;
}
.button{
  background: #E50914;
  border: none;
}
.ayuda{
  position: relative;
  margin-top: -4%;
  color: rgb(140, 140, 140);
}
.imagefc{
  position: relative;
  margin-top: -9%;

}
.iniciofc{
  position: relative;
  margin-top: -9.5%;
  color:rgba(114, 113, 113, 0.9);
  left: 5%;
  font-size: 13px;
}
h5{
margin-top: -3.9px;
font-weight: bold;
color: rgb(0, 0, 0);
}
#btonn{
  top: -30px;
  position: relative;
  background: rgb(255, 255, 255);
}
</style>
