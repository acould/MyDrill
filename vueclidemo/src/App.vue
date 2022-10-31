<template>
  <div id="app">
    <el-button type="success">成功按钮</el-button>
    <el-switch
      v-model="val"
      active-color="#13ce66"
      inactive-color="#ff4949"
      @change="gaibian"
    >
    </el-switch>
  </div>
</template>

<script>
export default {
  name: "app",
  components: {},
  data() {
    return {
      val: true,
    };
  },
  methods: {
    gaibian() {
      if (this.val == true) {
       let yes = (this.val = 1);
        console.log(yes, "哈哈");
      } else {
        console.log(2);
      }
    },
  },
  mounted() {},
};
</script>

<style>
</style>
