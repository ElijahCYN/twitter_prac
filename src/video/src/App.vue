<template>
  <div>
    <el-container>
      <el-header>
        <TopBar></TopBar>
      </el-header>
      <el-container>
        <!-- <el-aside width="300px">
          <LeftSideBar></LeftSideBar>
        </el-aside> -->
        <el-main>
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<style lang="scss" scoped>
@import "./assets/scss/main.scss";

.el-header {
  padding: 0;
}

.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: start;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
}

.el-main {
  // background-color: #e9eef3;
  color: #333;
  text-align: start;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>

<script>
import LeftSideBar from "./components/LeftBar.vue";
import TopBar from "./components/TopBar.vue";
import axios from "axios";

export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    LeftSideBar,
    TopBar,
  },
  methods: {
    checkJWT() {
      if (localStorage.token) {
        axios.defaults.headers.common[
          "Authorization"
        ] = `Bearer ${localStorage.token}`;
      }
    },
  },
  mounted() {
    this.checkJWT();
  },
};
</script>
