<script>
import CardComponent from "./CardComponent.vue";

export default {
  name: "MainComponent",
  components: { CardComponent },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="margin-top d-flex wrap">
        <!-- First article -->
        <CardComponent />
        <!--  FINE First article -->
      </div>
    </div>
  </main>
</template>
