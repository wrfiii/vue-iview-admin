<template>
  <div class="topBar"></div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class extends Vue {}
</script>

<style scoped lang='scss'>
.topBar {
  height: 50px;
  background: #ccc;
  position: fixed;
  width: 100vw;
  padding-left: 200px;
  top: 0;
}
</style>