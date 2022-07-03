<template>
  <el-container>
    <el-aside width="200px">
      <MenuTree />
    </el-aside>
    <el-main>Main</el-main>
  </el-container>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import MenuTree from "@/components/MenuTree.vue";

@Options({
  components: {
    MenuTree,
  },
})
export default class ContainerView extends Vue {}
</script>
