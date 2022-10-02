<template>
  <router-view class="bg" />
</template>

<script setup lang="ts"></script>
<style lang="scss">
.bg {
  background-color: $bg;
  color: $text-color;
}
* {
  &:hover {
    border: 0.5px solid red;
  }
}
</style>
