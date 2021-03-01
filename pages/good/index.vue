<template>
  <div>
    <h2>商品列表</h2>
    <div>
      <li
        v-for="item in productList"
        :key="item.id"
      >
        <nuxt-link :to="{path:'/good/'+item.id,query:{'name':item.name}}">{{item.name}}</nuxt-link>
      </li>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      productList: [
        { id: '1', name: '产品1' },
        { id: '2', name: '产品2' },
        { id: '3', name: '产品3' },
        { id: '4', name: '产品4' },
        { id: '5', name: '产品5' },
        { id: '6', name: '产品6' },
      ]
    }
  },

}
</script>

<style>
</style>