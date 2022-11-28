<template>
  <div class="relative bg-dark-blue w-[400px] lg:w-[900px] max-w-[1200px] h-[650px] max-h-[800px] rounded-3xl grid grid-cols-1 lg:grid-cols-2 p-2">
    <div class="bg-no-repeat bg-cover bg-center rounded-l-3xl w-full h-full image-card hidden lg:block"></div>
    <login-form></login-form>
    <floating-sign-in></floating-sign-in>
  </div>
</template>
<script>
import LoginForm from './LoginForm.vue'
import FloatingSignIn from './FloatingSignInCard.vue'

export default {
  name: "LoginCard",
  components: {
    LoginForm,
    FloatingSignIn
  }
}
</script>
<style scoped>
  .image-card {
    background-image: url('../assets/luoyi.png');
  }
</style>