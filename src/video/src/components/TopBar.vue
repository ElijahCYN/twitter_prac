<template>
  <el-menu class="el-menu-demo" mode="horizontal">
    <router-link to="/Home">
      <el-menu-item> Home </el-menu-item>
    </router-link>
    <router-link to="/Profile">
      <el-menu-item>Profile</el-menu-item>
    </router-link>
    <router-link to="/Posts">
      <el-menu-item>Posts</el-menu-item>
    </router-link>
  </el-menu>
</template>

<script>
export default {
  name: "LeftBar",
  props: {},
};
</script>

<style lang="scss" scoped>
a {
  text-decoration: none;
}

.el-menu {
  height: 100%;
  background: #b3c0d1;
}

.el-menu-item {
  height: 100%;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  font-size: 16px;
}

.el-menu-item.is-active {
  color: var(--el-color-black);
}
</style>
