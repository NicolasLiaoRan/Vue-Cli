<template>
  <div>
    <h1>hello from info component</h1>
    <button type="button" @click="add()">添加</button>
  </div>
</template>

<script>
export default {
  name:'info',
  methods:{
    add(){
      console.log("add event")
    }
  }
}
</script>

<style lang="stylus" scoped>

</style>