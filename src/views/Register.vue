<template>
  <div class="bg-no-repeat bg-cover bg-center image-card w-full flex items-center justify-center h-screen">
    <register-card></register-card>
  </div>
</template>
<script>
import RegisterCard from '../components/RegisterCard.vue'

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Register",
  components: {
    RegisterCard
  }
}
</script>

<style scoped>
  .image-card {
    background-image: url('../assets/bg-luoyi.png');
  }
</style>