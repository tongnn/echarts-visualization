<template>
  <div class="box">
    <panel-group />
    <pie></pie>

  </div>
</template>

<script>

import PanelGroup from './components/PanelGroup'
import pie from "./components/pie.vue"
// import chartsArr from '../../mixin/chartsArr'
export default {
  // mixins:[chartsArr],
   components: {
    PanelGroup,
    pie,
  },
  props: {
    className: {
      type: String,
      default: 'chart'
    },
    width: {
      type: String,
      default: '100%'
    },
    height: {
      type: String,
      default: '200px'
    }
  },
  data() {
    return {
      chart: null
    }
  },
  
}
</script>
<style lang="less" scoped>
.box{
  width: 100%;
  height: 100%;
  background: #1f2241;
}
</style>
