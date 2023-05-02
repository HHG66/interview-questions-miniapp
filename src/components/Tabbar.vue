<!--
 * @Author: HHG
 * @Date: 2023-05-02 09:46:56
 * @LastEditTime: 2023-05-02 09:48:17
 * @LastEditors: 韩宏广
 * @FilePath: \interview\src\components\Tabbar.vue
 * @文件说明: 底部导航栏组件
-->
<script setup>
import { Home, Category, Find, Cart, My } from '@nutui/icons-vue';
function tabSwitch(item, index) {
  console.log(item, index);
}
</script>

<template>
  <nut-tabbar @tab-switch="tabSwitch">
    <nut-tabbar-item tab-title="标签">
      <template #icon>
        <Home></Home>
      </template>
    </nut-tabbar-item>
    <nut-tabbar-item tab-title="标签">
      <template #icon>
        <Category></Category>
      </template>
    </nut-tabbar-item>
    <nut-tabbar-item tab-title="标签">
      <template #icon>
        <Find></Find>
      </template>
    </nut-tabbar-item>
    <nut-tabbar-item tab-title="标签">
      <template #icon>
        <Cart></Cart>
      </template>
    </nut-tabbar-item>
    <nut-tabbar-item tab-title="标签">
      <template #icon>
        <My></My>
      </template>
    </nut-tabbar-item>
  </nut-tabbar>
</template>

<style></style>