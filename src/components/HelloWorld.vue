<template>
 <div class="containere">
   <div class="transparecia">
    <arriba/>
    <abajo/>
   </div>
 </div>
</template>

<script>
import arriba from '@/components/arriba.vue'
import abajo from '@/components/abajo.vue'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    // eslint-disable-next-line vue/no-unused-components
    arriba,
    // eslint-disable-next-line vue/no-unused-components
    abajo
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.containere{
  min-height: 100vh;
  background-image: url('../assets/AR-es-20200210-popsignuptwoweeks-perspective_alpha_website_small.jpg')
}
.transparecia{
  background-color: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 170vh;
}
</style>
