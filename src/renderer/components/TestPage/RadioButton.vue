<template>
  <div>
    <el-radio v-model="radio" label="1">备选项</el-radio>
    <el-radio v-model="radio" label="2">备选项</el-radio>

    <el-radio-group v-model="radio0">
      <el-radio :label="3">备选项</el-radio>
      <el-radio :label="6">备选项</el-radio>
      <el-radio :label="9">备选项</el-radio>
    </el-radio-group>

    <div>
      <el-radio-group v-model="radio1">
        <el-radio-button label="上海"></el-radio-button>
        <el-radio-button label="北京"></el-radio-button>
        <el-radio-button label="广州"></el-radio-button>
        <el-radio-button label="深圳"></el-radio-button>
      </el-radio-group>
    </div>
    <div style="margin-top: 20px">
      <el-radio-group v-model="radio2" size="medium">
        <el-radio-button label="上海"></el-radio-button>
        <el-radio-button label="北京"></el-radio-button>
        <el-radio-button label="广州"></el-radio-button>
        <el-radio-button label="深圳"></el-radio-button>
      </el-radio-group>
    </div>
    <div style="margin-top: 20px">
      <el-radio-group v-model="radio3" size="small">
        <el-radio-button label="上海"></el-radio-button>
        <el-radio-button label="北京" disabled></el-radio-button>
        <el-radio-button label="广州"></el-radio-button>
        <el-radio-button label="深圳"></el-radio-button>
      </el-radio-group>
    </div>
    <div style="margin-top: 20px">
      <el-radio-group v-model="radio4" disabled size="mini">
        <el-radio-button label="上海"></el-radio-button>
        <el-radio-button label="北京"></el-radio-button>
        <el-radio-button label="广州"></el-radio-button>
        <el-radio-button label="深圳"></el-radio-button>
      </el-radio-group>
    </div>

    <div>
      <el-radio v-model="radio5" label="1" border>备选项1</el-radio>
      <el-radio v-model="radio5" label="2" border>备选项2</el-radio>
    </div>
    <div style="margin-top: 20px">
      <el-radio v-model="radio6" label="1" border size="medium">备选项1</el-radio>
      <el-radio v-model="radio6" label="2" border size="medium">备选项2</el-radio>
    </div>
    <div style="margin-top: 20px">
      <el-radio-group v-model="radio7" size="small">
        <el-radio label="1" border>备选项1</el-radio>
        <el-radio label="2" border disabled>备选项2</el-radio>
      </el-radio-group>
    </div>
    <div style="margin-top: 20px">
      <el-radio-group v-model="radio8" size="mini" disabled>
        <el-radio label="1" border>备选项1</el-radio>
        <el-radio label="2" border>备选项2</el-radio>
      </el-radio-group>
    </div>

    <div>
      <div>
        <el-checkbox v-model="checked1" label="备选项1" border></el-checkbox>
        <el-checkbox v-model="checked2" label="备选项2" border></el-checkbox>
      </div>
      <div style="margin-top: 20px">
        <el-checkbox v-model="checked3" label="备选项1" border size="medium"></el-checkbox>
        <el-checkbox v-model="checked4" label="备选项2" border size="medium"></el-checkbox>
      </div>
      <div style="margin-top: 20px">
        <el-checkbox-group v-model="checkboxGroup1" size="small">
          <el-checkbox label="备选项1" border></el-checkbox>
          <el-checkbox label="备选项2" border disabled></el-checkbox>
        </el-checkbox-group>
      </div>
      <div style="margin-top: 20px">
        <el-checkbox-group v-model="checkboxGroup2" size="mini" disabled>
          <el-checkbox label="备选项1" border></el-checkbox>
          <el-checkbox label="备选项2" border></el-checkbox>
        </el-checkbox-group>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
          checkboxGroup1: [],
        checkboxGroup2: [],
         checked1: true,
        checked2: false,
        checked3: false,
        checked4: true,
      radio: "1",
      radio0: "3",
      radio1: "上海",
      radio2: "上海",
      radio3: "上海",
      radio4: "上海",
      radio5: "1",
      radio6: "1",
      radio7: "1",
      radio8: "1",
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

