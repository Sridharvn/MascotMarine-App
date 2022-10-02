<template>
  <div class="body">
    <div class="body__details">
      <landing-text></landing-text>
    </div>
    <q-img
      src="./../assets/blur_edges-Increased-Blur-pexels-mudassir-ali-1556991.png"
      class="body__aside"
    ></q-img>
  </div>
</template>
<style lang="scss" scoped>
.body {
  display: flex;
  justify-content: center;
  &__aside {
    filter: blur(0.1px);
    width: 50vw;
    height: 100vh;
    mix-blend-mode: lighten;
    box-shadow: 0 0 8px 8px $bg inset;
  }
  &__details {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
<script lang="ts" setup>
import { onMounted } from "vue";
import LandingText from "src/components/LandingText.vue";

onMounted(function () {
  console.log("Test");
});
</script>
