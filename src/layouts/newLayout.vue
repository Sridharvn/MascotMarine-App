<template>
  <q-layout view="hhh lpR fff">
    <q-header class="header">
      <q-toolbar>
        <q-toolbar-title class="header__title">
          <q-avatar rounded>
            <img src="./../assets/mascotmarineLogo-Edited.png" class="header__image" />
          </q-avatar>
          Mascot Marine
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

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
  &__image {
  }
  &__title {
    color: $text-color;
    font-size: xx-large;
  }
}
</style>
