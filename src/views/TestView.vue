<template>
  <div class="test">
    <img src="../assets/logo.png" />
    <Test msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Test from "@/components/Test.vue";

@Options({
  components: {
    Test,
  },
})
export default class TestView extends Vue {}
</script>
