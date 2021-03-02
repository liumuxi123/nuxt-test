<template>
  <div>
    <h2>个人信息</h2>
    <div>{{sex}}</div>
  </div>
</template>

<script>
export default {
  middleware:'auth',
  data() {
    return {
      sex: '女'
    }
  },

}
</script>

<style>
</style>