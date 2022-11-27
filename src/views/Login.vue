<template>
  <div class="flex items-center justify-center h-screen">
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