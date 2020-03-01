<template>
<div class="containere">
    <div class="transparecia">
        <div class="Login">
            <arribaLogin/>
            <abajoLogin/>
        </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import arribaLogin from '@/components/arribaLogin.vue'
import abajoLogin from '@/components/abajoLogin.vue'
export default {
  name: 'Login',
  components: {
    arribaLogin,
    abajoLogin
  }
}
</script>
