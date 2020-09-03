<template>
  <div class="layout">
    <Layout />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Layout from "@/component/layout/index.vue";

@Component({
  components: { Layout }
})
export default class extends Vue {}
</script>

<style scoped>
.layout{
  width: 100%;
  height: 100%;
}
</style>