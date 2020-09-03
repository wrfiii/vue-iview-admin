<template>
  <div class="aside">
    <Menu :theme="theme2" accordion width="100%">
      <Submenu name="1">
        <template slot="title">
          <Icon type="ios-paper" />内容管理
        </template>
        <MenuItem name="1-1">文章管理</MenuItem>
        <MenuItem name="1-2">评论管理</MenuItem>
        <MenuItem name="1-3">举报管理</MenuItem>
      </Submenu>
      <Submenu name="2">
        <template slot="title">
          <Icon type="ios-people" />用户管理
        </template>
        <MenuItem name="2-1">新增用户</MenuItem>
        <MenuItem name="2-2">活跃用户</MenuItem>
      </Submenu>
    </Menu>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import { Menu, MenuItem, MenuGroup, Submenu, Icon } from "view-design";
@Component({
  components: {
    Menu,
    MenuItem,
    MenuGroup,
    Submenu,
    Icon
  }
})
export default class extends Vue {
  readonly theme2 = "dark";
}
</script>

<style scoped lang='scss'>
.aside {
  width: 200px;
  height: 100%;
  background-color: #515a6e;
}
</style>