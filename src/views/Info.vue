<template>
  <div>
    <h1>hello from info component</h1>
    <button type="button" @click="add()">添加</button>
  </div>
</template>

<script>
import store from '@/store'
export default {
  name:'info',
  store,
  methods:{
    add(){
      console.log("add event")
      store.commit('increase')
    }
  }
}
</script>

<style lang="stylus" scoped>

</style>