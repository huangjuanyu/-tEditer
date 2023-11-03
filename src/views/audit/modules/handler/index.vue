<!--
 * @Author: hjy zt17257@zongteng.net
 * @Date: 2023-11-02 17:04:44
 * @LastEditors: hjy zt17257@zongteng.net
 * @LastEditTime: 2023-11-03 15:48:37
 * @FilePath: /editor/src/views/audit/modules/handler/index.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <div class="handler">
    <!-- <XhEditor v-model="value" /> -->
    <sandBox />
  </div>
</template>

<script>
import sandBox from '../sandBox/index'
export default {
  components: {
    sandBox
  },
  props: {
    reachBottom: {
      type: Boolean,
      default: false
    }
  },
  data: () => ({
    value: ''
  }),
  methods: {
  }
}
</script>

<style lang="less">
.handler{
  position: fixed;
  padding: 7px 20px;
  background-color: #fff;
  width: 100%;
  bottom: 0;
  left: 0;
  box-shadow: 1px 1px 5px rgba(0, 0, 0, 0.118);
}
</style>
