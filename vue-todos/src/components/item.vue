<template>
  <div class="list-item editingClass editing">
    <label class="checkbox">
      <input type="checkbox" v-model="item.checked"/>
      <span class="checkbox-custom"></span>
    </label>
    <input type="text" v-model="item.text" placeholder="写点什么。。。"/>
    <a class="delete-item">
      <span class="icon-trash"></span>
    </a>
  </div>
</template>

<script>
  export default {
    // 子组件显式的用 props 选项声明它期待获得的数据，这里申明 它想要一个叫做 ’item‘的数据。
    props: ['item']
  }
</script>

<style lang="less">
  @import "../common/style/list-items.less";
</style>
