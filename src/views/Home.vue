<template>
  <div class="l_container">
    <div class="l_title">樓盤信息</div>
    <div class="l_card">
      <el-row :gutter="12">
        <el-col :span="6">
          <el-card shadow="always"><img src="" alt="" srcset=""></el-card>
        </el-col>
        <el-col :span="6">
          <el-card shadow="always"><img src="" alt="" srcset=""></el-card>
        </el-col>
        <el-col :span="6">
          <el-card shadow="always"><img src="logo" alt="" srcset=""></el-card>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.l_container {
  width: 100%;
  height: 500px;
  box-sizing: border-box;
  border: 1px solid pink;
  margin: 0 auto;
  .l_title{
    margin: 20px 0px;
    color: #999999;
    padding: 5px 0px;
    background-color: #f5f5f5;
    border-radius: 5px;
  }
  .l_card {
    .el-row {
      display: flex;
      justify-content: center;
    }
  }
}
</style>
