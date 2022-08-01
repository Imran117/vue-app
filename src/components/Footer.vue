<template>
  <footer class="footer">
    <div class="container footer__content">
      <h3 class="footer__content">Umurzakhov_dev</h3>
      <ul class="footer__content-list">
        <li v-for="(item, index) in icons" :key="index">
          <a :href="item.url">
            <img :src="item.img" alt="" />
          </a>
        </li>
      </ul>
      <p class="footer__content-sub">All Rights Reserved 2022 Imran</p>
    </div>
  </footer>
</template>

<script>
import { configIcon } from "@/_config";
export default {
  name: "Footer-vue",
  data() {
    return {
      icons: configIcon,
    };
  },
};
</script>

<style>
</style>