<template>
  <div class="bg-no-repeat bg-cover bg-center image-card w-full flex items-center justify-center h-screen">
    <login-card></login-card>
  </div>
</template>
<script>
import LoginCard from '../components/LoginCard.vue'

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Login",
  components: {
    LoginCard
  }
}
</script>

<style scoped>
  .image-card {
    background-image: url('../assets/bg-luoyi.png');
  }
</style>