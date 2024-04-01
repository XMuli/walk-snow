<template>
    <div id="MainWindows">
        <el-radio-group v-model="tabPosition" style="margin-bottom: 30px;">
            <el-radio-button label="top">top</el-radio-button>
            <el-radio-button label="right">right</el-radio-button>
            <el-radio-button label="bottom">bottom</el-radio-button>
            <el-radio-button label="left">left</el-radio-button>
        </el-radio-group>

        <el-tabs :tab-position="tabPosition" style="height: 200px;">
            <el-tab-pane label="OCR 提取文字"><OCRComponents/></el-tab-pane>
            <el-tab-pane label="Image Translate 图片翻译"></el-tab-pane>
            <el-tab-pane label="Text to Speech 文本转语音"></el-tab-pane>
            <el-tab-pane label="Speech to text 语音转文本"></el-tab-pane>
        </el-tabs>
    </div>
</template>

<script>
import OCRComponents from './OCR.vue'
  export default {
    components: {
        OCRComponents
    },
    data() {
      return {
        tabPosition: 'left'
      };
    }
  };
</script>

<style scoped>
/* Your component-specific styles here */
</style>