<template>
  <header-component/>
  <welcome-component/>
  <footer-component/>
</template>

<script>
import FooterComponent from "@/components/FooterComponent.vue";
import HeaderComponent from "@/components/HeaderComponent.vue";
import WelcomeComponent from "@/components/WelcomeComponent.vue";

export default {
  name: "Home",
  components: {
    FooterComponent,
    HeaderComponent,
    WelcomeComponent
  }
}
</script>

<style lang="less" scoped>

</style>