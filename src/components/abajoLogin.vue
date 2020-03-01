<template>
<div class="card">
      <div class="pre">
        <h6>¿Preguntas? Llama al 800-345-1375</h6>
      </div>
        <div class="columns">
          <div class="column is-6">
            <h6>Terminos de tarjetas de regalo</h6>
          </div>
          <div class="column is-6">
            <h6>Terminos de uso</h6>
          </div>
          <div class="column is-5">
            <h6>Declaracion de privacidad</h6>
          </div>
        </div>
          <div class="field">
            <div class="control has-icons-left">
              <div class="select">
                <select style="background: rgba(0, 0, 0, 0.8); border-color: rgba(140, 140, 140, 0.6);">
                  <option selected>Español</option>
                  <option>Ingles</option>
                </select>
              </div>
              <div class="icon is-small is-left">
                <i class="fas fa-globe"></i>
              </div>
            </div>
          </div>
    </div>
</template>

<script>
export default {
  name: 'abajoLogin',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.card{
  background: rgba(0, 0, 0, 0.8);
  width: 100%;
  height: 36%;
  top: 134%;
  position: absolute;
}
.pre{
  position:absolute;
  color:rgb(140, 140, 140);
  top: 12%;
  left: 15%;
  font-size: 18px;
}
.column{
  color:rgb(140, 140, 140);
  font-size: 13px;
}
.columns{
  position:absolute;
  top: 33%;
  left: 15%;
}
.field{
  position:absolute;
  top: 49%;
  left: 15%;
  background: rgba(0, 0, 0, 0.8);
}
</style>
