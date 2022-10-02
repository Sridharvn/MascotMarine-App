<template>
  <q-layout view="hhh lpR fff">
    <q-header class="header">
      <q-toolbar>
        <q-toolbar-title class="header__title">
          <q-avatar rounded>
            <img src="./../assets/mascotmarineLogo-Edited.png" class="header__image" />
          </q-avatar>
          Mascot Marine
          <p class="header__undertitle">
            Mascot Marine Services, Keilor East, Melbourne, Australia
          </p>
        </q-toolbar-title>
        <!-- <q-space> </q-space> -->
      </q-toolbar>
      <q-space></q-space>
      <header-links :drawerRight="drawerRight"></header-links>
      <q-btn
        flat
        @click="drawerRight = !drawerRight"
        dense
        icon="menu"
        class="header__drawerbutton"
      />
    </q-header>
    <!-- <q-drawer
      side="right"
      v-model="drawerRight"
      show-if-above
      bordered
      :width="200"
      :breakpoint="500"
      class="header__drawer-right"
    >
      <q-scroll-area class="fit">
        <div class="q-pa-sm">
          <div v-for="n in 50" :key="n">Drawer {{ n }} / 50</div>
        </div>
      </q-scroll-area>
    </q-drawer> -->
    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="footer"> CyberNet Developers </q-footer>
  </q-layout>
</template>
<style lang="scss" scoped>
.footer {
  color: $text-color;
  text-align: center;
}
.header {
  height: 10vh;
  display: flex;
  &__undertitle {
    font-size: small;
    margin-left: 20px;
  }
  &__drawerbutton {
    margin-bottom: 17px;
  }
  &__image {
  }
  &__title {
    color: $text-color;
    font-size: xx-large;
  }

}
</style>
<script lang="ts" setup>
import HeaderLinks from "src/components/HeaderLinks.vue";
import { ref } from "vue";
var drawerRight = ref(false);
</script>
