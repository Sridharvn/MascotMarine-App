<!-- eslint-disable vue/no-mutating-props -->
<template>
  <div class="body">
    <div class="body__links">
      <q-item
        v-for="link in LinkList"
        :key="link.link"
        to="{{link.link}}"
        class="body__list-items"
      >
        {{ link.title }}
      </q-item>
    </div>
    <q-drawer
      side="right"
      v-model="drawerRight"
      :width="200"
      :breakpoint="500"
      class="body__drawer-right"
    >
      <q-scroll-area class="fit body__drawer-right">
        <div class="q-pa-sm">
          <q-item v-for="link in LinkList" to="{{link.link}}" :key="link.link">{{
            link.title
          }}</q-item>
        </div>
      </q-scroll-area>
    </q-drawer>
  </div>
</template>
<style lang="scss" scoped>
.body {
  &__links {
    list-style-type: none;
    width: max-content;
    display: flex;
    flex-direction: row;
    gap: 1;
    font-size: x-large;
    color: $text-color;
    margin-top: 10px;
  }
  &__list-items {
    padding: 10px;
    &:last-child {
      margin-right: 10px;
    }
  }
  &__drawer-right {
    background-color: $secondary;
    color: $text-color;
  }
}
</style>
<script lang="ts" setup>
defineProps<{
  drawerRight?: boolean;
}>();
const LinkList = [
  {
    title: "Home",
    link: "/",
  },
  {
    title: "Service List",
    link: "/services",
  },
  {
    title: "Contact Us",
    link: "/contactus",
  },
  {
    title: "About Us",
    link: "/aboutus",
  },
  {
    title: "Products",
    link: "/products",
  },
  {
    title: "Related Links",
    link: "/relatedlinks",
  },
];
</script>
