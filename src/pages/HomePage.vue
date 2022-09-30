<script lang="ts" setup>
import { onMounted } from "vue";

onMounted(function () {
  console.log("Test");
});
</script>
<template>
  <div class="body">
    <div class="body__details">
      <p class="body__text">
        Melbourne-based Marine Consultancy Company, providing marine expertise to the
        shipping community. Independent surveys. Authorised surveyor for Honduran and
        Bolivian Flag vessels. Authorised PMDS surveyor for Geelong and Melbourne
        (Panamanian Maritime documentation services). Authorised Technical/Engineering
        surveyor for Intertek Australia.
      </p>
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
  &__text {
    width: 50vw;
    font-size: x-large;
    padding: 10px;
  }
}
</style>
