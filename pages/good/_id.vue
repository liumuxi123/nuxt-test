<template>
  <div>
    <h2>商品详情</h2>
    <div>{{name}}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: ''
    }
  },
  created() {
  },
  mounted(){
    this.name = this.$route.query.name
  }
}
</script>

<style>
</style>