<template>
  <div>Home</div>
  <HelloWorld msg="msg" />
</template>
<script lang="ts">
  import { ref } from 'vue'
  import HelloWorld from '../components/HelloWorld.vue'

  export default {
    name: 'Home',
    components: {
      HelloWorld
    },
    setup() {
      const msg = ref('')
      const message = 'ssss'
      console.log(message)
      msg.value = 'Hello in the World'
      // 测试提交
      const jumpTest = (x: any, y: any) => {
        return x + y
      }
      // 添加注释
      console.log(jumpTest(1, 2), 'jumpTest')
    }
  }
</script>
