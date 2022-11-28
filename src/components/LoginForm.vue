<template>
  <div class="flex flex-col justify-center px-6 lg:pl-6 lg:pr-12">
    <h2 class="text-left text-3xl text-light-green font-[800] mb-10">Lets get Started</h2>
    <form class="flex flex-col" action="">
      <div class="flex flex-col space-y-6">
        <input class="border text-white font-[700] border-opacity-50 border-light-green bg-transparent px-4 py-2 rounded-lg focus:outline-none" type="email" placeholder="Masukkan Email">
        <div class="border border-light-green flex items-center w-full text-white font-[700] border-opacity-50 rounded-lg">
          <input class="bg-transparent px-4 py-2 flex-grow focus:outline-none" :type="passwordFieldType" placeholder="Masukkan Password">
          <font-awesome-icon class="text-white hover:cursor-pointer mx-4" :icon="passwordIcon" @click="swithVisibility" />
        </div>
        <span class="text-center text-sm text-white text-opacity-60 font-[700]">
          By continuing you agree to 
          <a class="text-light-green font-[800]" href="#">Term &amp; Conditions</a>
          and
          <a class="text-light-green font-[800]" href="#">Privacy Policy</a>
        </span>
      </div>
      <button class="w-full bg-light-green hover:bg-green-500 text-white h-11 rounded-lg mt-14" type="submit">Create Account</button>
    </form>
    <span class="text-center text-sm text-white text-opacity-60 font-[700] mt-2">
      Already have an account?
      <a class="text-light-green font-[800]" href="#">Login now</a>
    </span>
  </div>
</template>
<script>
export default {
  name: "LoginForm",
  data() {
    return {
      password: "",
      passwordFieldType: "password",
      passwordIcon: "fa-solid fa-eye-slash"
    }
  },
  methods: {
    swithVisibility() {
      this.passwordFieldType = this.passwordFieldType === "password" ? "text" : "password"
      this.passwordIcon = this.passwordIcon === "fa-solid fa-eye-slash" ? "fa-solid fa-eye" : "fa-solid fa-eye-slash"
    }
  }
}
</script>