<template>
  <div>
    <!--抽屉按钮-->
    <!--
    <el-button @click="drawer = true"  type="primary" style="margin-right: 16px;">点我打开</el-button>

    <el-drawer title="我是标题" :visible.sync="drawer" direction="ltr" :before-close="handleClose">
        <NavMenu></NavMenu>   
    </el-drawer>
    -->


  </div>
</template>

<script>
import NavMenu from "./Main/LeftContent";

export default {
  components: { NavMenu },

  data() {
    return {
      drawer: false
    };
  }
};
</script>