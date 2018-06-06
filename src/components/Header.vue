<template>
  <div class="header">
    <el-menu :default-active="$route.path" class="el-menu-demo" mode="horizontal" @select="handleSelect">
      <el-menu-item index="/">首页</el-menu-item>
      <el-menu-item index="/map">地图</el-menu-item>
    </el-menu>
  </div>
</template>


<script>
export default {
  name: 'HomeHeader',
  data() {
    return {

    }
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(keyPath);
      this.$router.push(key);
    }
  }

}

</script>

<style lang="stylus" scoped>

</style>
