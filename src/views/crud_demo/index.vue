<template>
  <div>
    <el-radio v-model="radio" label="1">备选项</el-radio>
    <el-radio v-model="radio" label="2">备选项</el-radio>
    <el-time-picker
      v-model="value1"
      :picker-options="{
      selectableRange: '18:30:00 - 20:30:00'
    }"
      placeholder="任意时间点">
    </el-time-picker>
    <el-time-picker
      arrow-control
      v-model="value2"
      :picker-options="{
      selectableRange: '18:30:00 - 20:30:00'
    }"
      placeholder="任意时间点">
    </el-time-picker>
  </div>
</template>

<script>
export default {
  data () {
    return {
      radio: '1',
      value1: new Date(2016, 9, 10, 18, 40),
      value2: new Date(2016, 9, 10, 18, 40)
    }
  }
}
</script>
