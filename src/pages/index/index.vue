<template>
  <view class="index">
    <!-- <Counter /> -->
    <div class="header"></div>
    <div class="container"></div>
    <nut-tabbar bottom safe-area-inset-bottom placeholder>
      <nut-tabbar-item v-for="(item, index) in List" :tab-title="item.title" :icon="item.icon"> </nut-tabbar-item>
    </nut-tabbar>

  </view>
</template>

<script>
import { h } from 'vue';
import './index.less'
// import Counter from '../../components/Counter.vue'
import Tabbar from '../../components/Tabbar.vue'
import { Home, Category, Find, Cart, My } from '@nutui/icons-vue';

export default {
  name: 'Index',
  components: {
    // Counter
    Tabbar
  },
  setup() {
    const List = [
      {
        title: '首页',
        icon: h(Home),
      },
      {
        title: '题库',
        icon: h( Find),
      },
      {
        title: '我的',
        icon: h(My),

      },
      {
        title: '关于',
        icon: h(Category),
      },
    ]
    return {
      List,
    };
  },
}
</script>
 
