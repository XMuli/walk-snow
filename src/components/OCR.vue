<template>
    <div >
        <el-select v-model="value" placeholder="请选择">
    <el-option
      v-for="item in options"
      :key="item.value"
      :label="item.label"
      :value="item.value"
      :disabled="item.disabled">
    </el-option>
  </el-select>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        options: [{
          value: '选项1',
          label: '线路1: 百度'
        }, {
          value: '选项2',
          label: '线路2: 有道',
          disabled: true
        }],
        value: '线路1: 百度'
      }
    }
  }
</script>

<style scoped>
/* Your component's CSS styles go here */
</style>