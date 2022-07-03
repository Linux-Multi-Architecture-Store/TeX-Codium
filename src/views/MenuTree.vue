<template>
  <el-menu>
    <el-menu-item index="1-1">
      <router-link to="/test"><div class="el-icon-info"></div></router-link>
    </el-menu-item>
    <el-menu-item index="1-2">选项2</el-menu-item>
  </el-menu>
</template>

<script lang="ts">
import { Vue } from "vue-class-component";

export default class MenuTree extends Vue {}
</script>
