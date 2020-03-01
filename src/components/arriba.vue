<template>
  <div>
    <div class="columns">
      <div class="column">
                  <section class="hero">
                    <div class="hero-body">
                      <img class="tamaño" src="../assets/Logo_Netflix.png" alt="">
                    </div>
                  </section>
                <div class="column">
                   <div class="control">
                      <button @click="login" style="background: #E50914; border: none; left: 88%; top: -82px; color:aliceblue;" class="button">iniciar sesion</button>
                    </div>
                </div>
        </div>
    </div>
    <div>
      <div style=" left: 22%;" class="container">
        <h1 style="color:antiquewhite; left: 50%; width: 550px;" class="title is-1">
          Programas y peliculas sin limite y mucho mas.
        </h1>
        <h1>
          Disfruta donde quieras. Cancela en cualquier momento.
        </h1>
      </div>
    </div>
        <div class="field has-addons">
          <div style="top: 70px; left: 30%; " class="control">
            <input class="input is-large" type="text" placeholder="Find a repository">
          </div>
          <div style="top: 70px; left: 30%;" class="control">
            <a style="background: #E50914;" class="button is-info is-large">
              PROBAR AHORA >
            </a>
          </div>
        </div>
  </div>
</template>

<script>
export default {
  name: 'arriba',
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
  width: 140px;
  height: 80px;
  position:absolute;
  top: 0%;
  left: 3%;
}
h1{
  align-content: center;
}
</style>
