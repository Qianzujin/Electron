<!--
Author:Wangjj
QQ:738367869
Data:2020.1.19
-->
<template>
  <div>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--基本链接-->
    <el-row :gutter="10">
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link href="https://element.eleme.io" target="_blank">默认链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="primary">主要链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="success">成功链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="warning">警告链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="danger">危险链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="info">信息链接</el-link>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--不可用链接-->
    <el-row :gutter="10">
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link disabled>默认链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="primary" disabled>主要链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="success" disabled>成功链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="warning" disabled>警告链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="danger" disabled>危险链接</el-link>
      </el-col>
      <el-col :xs="4" :sm="4" :md="4" :lg="4" :xl="4">
        <el-link type="info" disabled>信息链接</el-link>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <!--有无下划线-->
    <el-row :gutter="10">
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-link :underline="false">无下划线</el-link>
      </el-col>
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-link>有下划线</el-link>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>
    <!--图标链接-->
    <el-row :gutter="10">
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-link icon="el-icon-edit">编辑</el-link>
      </el-col>
      <el-col :xs="12" :sm="12" :md="12" :lg="12" :xl="12">
        <el-link>
          查看
          <i class="el-icon-view el-icon--right"></i>
        </el-link>
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