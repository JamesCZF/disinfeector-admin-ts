<template>
  <div class="hello">
    {{msg}}{{red}}
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
enum colors  {
  red,
  green,
  blue
}
export default defineComponent({
  // 已启用类型推断
  setup() {
    let msg = 'hello world'
    return {
      msg,
      red: colors.red
    }
  },
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">

</style>
