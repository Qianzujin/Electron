<template>
  <!--登陆首页-->
  <!--页面粒子效果
  <vue-canvas-nest :config="{color:'255,0,0', count: 88}" :el="'#area'"></vue-canvas-nest>
  color：：画布线条颜色，默认值：'255,0,0'；颜色为(R，G，B)。
  opacity*行的不透明度(0~1)，默认值为：0.7.
  count*行数，默认值为：99.
  zIndex*z空间的索引，默认值：-1.
  -->
  <div>
    <vueCanvasNest :config="{color:'0,0,255', count: 88}"></vueCanvasNest>

    <div v-if="loginDisplay">
      <div class="center">
        <img class="logo" src="~@/assets/logo-electron.png" />
      </div>
      <div class="center font-mircroft-black-ex-large">
        <el-link type="primary" @click="login">Electron-Vue ElementUI Tool</el-link>
      </div>
    </div>

    <el-row :gutter="10" v-if="mainDisplay">
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <div class="grid-content">
          <img class="logo-small-left" src="~@/assets/logo-electron.png" />
        </div>
      </el-col>
      <el-col :xs="11" :sm="11" :md="11" :lg="11" :xl="11">
        <div class="grid-content">
          <div class="top-title">Electron-Vue ElementUI Tool</div>
        </div>
      </el-col>
      <el-col :xs="7" :sm="7" :md="7" :lg="7" :xl="7">
        <div class="grid-content">
          <el-input class="top-sereach" v-model="input" placeholder="搜索文档"></el-input>
        </div>
      </el-col>
    </el-row>
    <el-row :gutter="0" v-if="mainDisplay">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <div class="link-top"></div>
      </el-col>
    </el-row>
    <el-row :gutter="0" v-if="mainDisplay">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-tabs :tab-position="tabPosition" style="height: 100%;">
          <el-tab-pane label="Button 按钮">
              <ElementButtons></ElementButtons>
          </el-tab-pane>
          <el-tab-pane label="Link 文字链接">
            <ElementTextLinks></ElementTextLinks>
          </el-tab-pane>
          <el-tab-pane label="Radio 单选框">
            <ElementRadios></ElementRadios>
          </el-tab-pane>
          <el-tab-pane label="定时任务补偿">定时任务补偿</el-tab-pane>
          <el-tab-pane label="用户管理">用户管理</el-tab-pane>
          <el-tab-pane label="配置管理">配置管理</el-tab-pane>
          <el-tab-pane label="角色管理">角色管理</el-tab-pane>
          <el-tab-pane label="定时任务补偿">定时任务补偿</el-tab-pane>
          <el-tab-pane label="用户管理">用户管理</el-tab-pane>
          <el-tab-pane label="配置管理">配置管理</el-tab-pane>
          <el-tab-pane label="角色管理">角色管理</el-tab-pane>
          <el-tab-pane label="定时任务补偿">定时任务补偿</el-tab-pane>
        </el-tabs>
      </el-col>
    </el-row>
  </div>
</template>


<style scoped>
@import "./css/main.css";
@import "./css/font.css";

.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
</style>

<script>
/** 粒子效果组件注册 **/
import vueCanvasNest from "vue-canvas-nest";
/** 按钮注册 **/
import ElementButton from "./TestPage/Button";
import ElementButtons from "./controls/elementButton";
import ElementTextLinks from "./controls/elementTextLink";
import ElementRadios from "./controls/elementRadio";

export default {
  name: "login-page",
  components: {
    vueCanvasNest,
    ElementButton,
    ElementButtons,
    ElementTextLinks,
    ElementRadios
  },
  methods: {
    login() {
      this.loginDisplay = false;
      this.mainDisplay = true;
      this.$notify({
        title: "登陆成功",
        message: "Electron-Vue ElementUi Tool",
        position: "bottom-right"
      });
    },
    loginSuccessInfo() {
      this.$notify({
        title: "自定义位置",
        message: "右下角弹出的消息",
        position: "bottom-right"
      });
    },
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  },
  data() {
    return {
      loginDisplay: true,
      mainDisplay: false,
      tabPosition: "left",
      tabPaneDisabled: true,
      input: ""
    };
  }
};
</script>



<!-- 星空js
<template>
  <div class="home">
    <canvas id="canv"></canvas>
  </div>

</template>

<script>

  import {stars_nest} from '../../static/lqbz/stars-nest'

  export default {
    name: 'Home',
    data () {
      return {
      }
    },
    mounted(){//****在这里绑定监听器
      stars_nest();

    },
    methods: {


    }

  }
</script>
<style>
  html {
    height: 100%;
    background-image: -webkit-radial-gradient(ellipse farthest-corner at center top, #000d4d 0%, #000105 100%);
    background-image: radial-gradient(ellipse farthest-corner at center top, #000d4d 0%, #000105 100%);
    cursor: arrow;
  }

  body {
    width: 100%;
    margin: 0;
    overflow: hidden;
  }

</style>

-->