<template>
  <div>
    <h1>hello from info component</h1>
    <button
      type="button"
      @click="add()"
    >添加</button>
    <hr>
  </div>
</template>

<script>
import store from '@/store'
import axios from 'axios'
export default {
  name: 'info',
  store,
  methods: {
    add () {
      console.log("add event")
      store.commit('increase')
    }
  },
  created () {
    axios.get('http://localhost:6987/api/values').then((res) => {
      console.log(res.data)
    })
  }
}
</script>

<style lang="stylus" scoped></style>