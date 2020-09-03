<template>
  <div class="main">
    <Aside />
    <Topbar />
    <div class="container">
      我是路由
      <router-view></router-view>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

import Aside from "./aside/index.vue";

import Topbar from "./topbar/index.vue";

@Component({
  components: { Aside, Topbar }
})
export default class extends Vue {}
</script>

<style scoped lang='scss'>
.main {
  height: 100%;
  display: flex;
  .container {
    padding-top: 50px;
  }
}
</style>