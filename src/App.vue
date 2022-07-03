<template>
  <!--
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/test">Test</router-link> |
    <router-link to="/container">Container</router-link>
  </nav>
  <router-view />
  -->
  <el-container>
    <el-aside width="200px">
      <MenuTree />
    </el-aside>
    <el-main><router-view /></el-main>
  </el-container>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

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
