<template>
  <div class="test">
    <h1>{{ msg }}</h1>
    <el-empty></el-empty>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
  },
})
export default class Test extends Vue {
  msg!: string;
}
</script>
