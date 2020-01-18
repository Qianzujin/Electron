<template>
  <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="BUTTON" name="first">
      First
      <ElementButton></ElementButton>
    </el-tab-pane>
    <el-tab-pane label="Second" name="second">
      <ElementIcon></ElementIcon>
    </el-tab-pane>
    <el-tab-pane label="Third" name="third">
        <ElementTextLink></ElementTextLink>
    </el-tab-pane>
    <el-tab-pane label="Fourth" name="fourth">
        <ElementRadioButton></ElementRadioButton>
    </el-tab-pane>
    
    <el-tab-pane label="Fith" name="Fith">
        <ElementCheckBox></ElementCheckBox>
    </el-tab-pane>
  </el-tabs>
</template>
<script>
import ElementButton from "./TestPage/Button";
import ElementIcon from "./TestPage/Icon";
import ElementTextLink from "./TestPage/TextLink";
import ElementRadioButton from "./TestPage/RadioButton";
import ElementCheckBox from "./TestPage/CheckBox";


export default {
  data() {
    return {
      activeName: "first"
    };
  },
  components: { ElementButton, ElementIcon ,ElementTextLink ,ElementRadioButton,ElementCheckBox},
  methods: {
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
};
</script>