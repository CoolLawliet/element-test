<template>
  <div id="app">
    <el-tag>{{ msg }}</el-tag>
    <el-input v-model="msg" />
    <el-table :data="tableData" style="width: 100%">
      <el-table-column prop="date" label="日期" width="180"> </el-table-column>
      <el-table-column prop="name" label="姓名" width="180"> </el-table-column>
      <el-table-column prop="address" label="地址"> </el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      msg: "1",
      tableData: [
        { id: 1, name: "张三", age: 18, sex: "男" },
        { id: 2, name: "张s", age: 14, sex: "nan" },
        { id: 3, name: "张d", age: 138, sex: "nv" },
        { id: 4, name: "张f", age: 148, sex: "男" },
      ],
    };
  },
};
</script>

<style></style>
