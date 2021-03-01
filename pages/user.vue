<template>
  <div>
    <h2>个人中心页面</h2>
    <div>{{userName}}</div>
    <div>
      <nuxt-link to="/user/">信息</nuxt-link>
      <nuxt-link to="/user/favorite">爱好</nuxt-link>
    </div>
    <nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: '刘姥姥'
    }
  },

}
</script>

<style>
</style>