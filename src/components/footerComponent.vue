<template>
  <mt-tabbar class="component" :style="node.styl" v-model="selected">
    <mt-tab-item id="首页">
      首页
    </mt-tab-item>
    <mt-tab-item id="活动">
      活动
    </mt-tab-item>
    <mt-tab-item id="购物车">
      购物车
    </mt-tab-item>
    <mt-tab-item id="我的">
      我的
    </mt-tab-item>
  </mt-tabbar>
</template>

<script>
  import { Tabbar, TabItem } from 'mint-ui';
  export default {
    name: 'footerComponent',
    props: ['node', 'themeColor'],
    data(){
      return {
        selected:'首页'
      }
    },
    computed: {
    },
    methods:{

    },
    components:{
      'mtTabbar':Tabbar,
      'mtTabItem':TabItem
    }
  }
</script>

<style scoped>
  section {
    border: 2px solid transparent;
  }
  section:hover {
    border: 2px solid tomato;
  }
</style>
