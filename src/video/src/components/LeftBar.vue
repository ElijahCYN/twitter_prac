<template>
  <div class="info-content">
    <div class="demo-basic--circle">
      <div class="block">
        <el-avatar :size="100" :src="circleUrl"></el-avatar>
      </div>
      <div class="tag-content">
        <el-badge :value="12" class="item">
          <el-button size="small">comments</el-button>
        </el-badge>
        <el-badge :value="3" class="item" type="primary">
          <el-button size="small">replies</el-button>
        </el-badge>
        <el-badge :value="3" class="item" type="warning">
          <el-button size="small">replies</el-button>
        </el-badge>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LeftBar",
  props: {},
  data() {
    return {
      circleUrl:
        "https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png",
    };
  },
};
</script>

<style lang="scss" scoped>

.info-content {
  padding: 1rem .5rem;
}

.tag-content {
  margin: 1rem 0;
}

.item {
  margin-right: 1.5rem;
}
</style>