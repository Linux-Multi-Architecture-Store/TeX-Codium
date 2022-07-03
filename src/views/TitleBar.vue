<template>
  <el-row :gutter="20" type="flex" justify="center" align="middle">
    <el-col :span="4"
      ><div class="grid-content bg-purple"><div>TeX Codium</div></div></el-col
    >
    <el-col :span="16"><div class="grid-content bg-purple"></div></el-col>
    <el-col :span="4"><div class="grid-content bg-purple"></div></el-col>
  </el-row>
</template>

<style lang="scss">
.head_logo {
  height: 45px;
}
.el-col {
  border-radius: 4px;
}
.bg-purple-dark {
  background: #99a9bf;
}
.bg-purple {
  background: #d3dce6;
}
.bg-purple-light {
  background: #e5e9f2;
}
.grid-content {
  border-radius: 4px;
  min-height: 36px;
}
</style>
