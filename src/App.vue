<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: "MyApp",
  components: { HeaderComponent, MainComponent, FooterComponent },
};
</script>

<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>
