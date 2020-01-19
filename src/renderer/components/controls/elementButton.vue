<!--
Author:Wangjj
QQ:738367869
Data:2020.1.19
-->
<template>
  <div>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--基本按钮-->
    <el-row :gutter="10">
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button>默认按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary">主要按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="success">成功按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="info">信息按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="warning">警告按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="danger">危险按钮</el-button>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--禁用按钮-->
    <el-row :gutter="10">
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button disabled>默认按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary" disabled>主要按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="success" disabled>成功按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="info" disabled>信息按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="warning" disabled>警告按钮</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="danger" disabled>危险按钮</el-button>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--文字按钮-->
    <el-row :gutter="10">
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-button type="text">文字按钮</el-button>
      </el-col>
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-button type="text" disabled>文字按钮</el-button>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--图标按钮-->
    <el-row :gutter="10">
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary" icon="el-icon-edit"></el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary" icon="el-icon-share"></el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary" icon="el-icon-delete"></el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary" icon="el-icon-search">搜索</el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary">
          上传
          <i class="el-icon-upload el-icon--right"></i>
        </el-button>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-button type="primary">
          设置
          <i class="el-icon-setting el-icon--right"></i>
        </el-button>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--按钮组-->

    <el-row :gutter="10">
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-button-group>
          <el-button type="primary" icon="el-icon-arrow-left">上一页</el-button>
          <el-button type="primary">
            下一页
            <i class="el-icon-arrow-right el-icon--right"></i>
          </el-button>
        </el-button-group>
      </el-col>
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-button-group>
          <el-button type="primary" icon="el-icon-edit"></el-button>
          <el-button type="primary" icon="el-icon-share"></el-button>
          <el-button type="primary" icon="el-icon-delete"></el-button>
        </el-button-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--加载中-->
    <el-row :gutter="10">
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-button type="primary" :loading="true">加载中</el-button>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <!--不同尺寸-->
    <el-row :gutter="10">
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button>默认按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="medium">中等按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="small">小型按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="mini">超小按钮</el-button>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button round>默认按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="medium" round>中等按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="small" round>小型按钮</el-button>
      </el-col>
      <el-col :xs="6" :sm="6" :md="6" :lg="6" :xl="6">
        <el-button size="mini" round>超小按钮</el-button>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      electron: process.versions.electron,
      name: this.$route.name,
      node: process.versions.node,
      path: this.$route.path,
      platform: require("os").platform(),
      vue: require("vue/package.json").version
    };
  }
};
</script>