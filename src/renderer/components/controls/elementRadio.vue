<!--
Author:Wangjj
QQ:738367869
Data:2020.1.19
-->

<template>
  <div>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <!--单选框-->
    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio v-model="radio" label="1">备选项</el-radio>
        <el-radio v-model="radio" label="2">备选项</el-radio>
      </el-col>
    </el-row>

    <!--禁用单选框-->
    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio disabled v-model="radio1" label="禁用">备选项</el-radio>
        <el-radio disabled v-model="radio1" label="选中且禁用">备选项</el-radio>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <!--单选框组-->
    <!--
        结合el-radio-group元素和子元素el-radio可以实现单选组，在el-radio-group中绑定v-model，在el-radio中设置好label即可，无需再给每一个el-radio绑定变量，另外，还提供了change事件来响应变化，它会传入一个参数value。
    -->
    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radio2">
          <el-radio :label="3">备选项</el-radio>
          <el-radio :label="6">备选项</el-radio>
          <el-radio :label="9">备选项</el-radio>
        </el-radio-group>
      </el-col>
    </el-row>
    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <!--单选按钮样式-->
    <!--只需要把el-radio元素换成el-radio-button元素即可，此外，Element 还提供了size属性。-->
    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radioa">
          <el-radio-button label="上海"></el-radio-button>
          <el-radio-button label="北京"></el-radio-button>
          <el-radio-button label="广州"></el-radio-button>
          <el-radio-button label="深圳"></el-radio-button>
        </el-radio-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radiob" size="medium">
          <el-radio-button label="上海"></el-radio-button>
          <el-radio-button label="北京"></el-radio-button>
          <el-radio-button label="广州"></el-radio-button>
          <el-radio-button label="深圳"></el-radio-button>
        </el-radio-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radioc" size="small">
          <el-radio-button label="上海"></el-radio-button>
          <el-radio-button label="北京" disabled></el-radio-button>
          <el-radio-button label="广州"></el-radio-button>
          <el-radio-button label="深圳"></el-radio-button>
        </el-radio-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radiod" size="mini">
          <el-radio-button label="上海" disabled></el-radio-button>
          <el-radio-button label="北京" disabled></el-radio-button>
          <el-radio-button label="广州" disabled></el-radio-button>
          <el-radio-button label="深圳" disabled></el-radio-button>
        </el-radio-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio v-model="radio3" label="1" border>备选项1</el-radio>
        <el-radio v-model="radio3" label="2" border>备选项2</el-radio>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio v-model="radio4" label="1" border size="medium">备选项1</el-radio>
        <el-radio v-model="radio4" label="2" border size="medium">备选项2</el-radio>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-col :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
        <el-radio-group v-model="radio5" size="small">
          <el-radio label="1" border>备选项1</el-radio>
          <el-radio label="2" border disabled>备选项2</el-radio>
        </el-radio-group>
      </el-col>
    </el-row>

    <!--分割线-->
    <el-row :gutter="10" style="margin-bottom:10px;"></el-row>

    <el-row :gutter="10">
      <el-radio-group v-model="radio6" size="mini" disabled>
        <el-radio label="1" border>备选项1</el-radio>
        <el-radio label="2" border>备选项2</el-radio>
      </el-radio-group>
    </el-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      radio: "1",
      radio1: "选中且禁用",
      radio2: "3",
      radio3: "1",
      radio4: "1",
      radio5: "1",
      radio6: "1",
      radioa: "上海",
      radiob: "上海",
      radioc: "上海",
      radiod: "上海"
    };
  }
};
</script>
