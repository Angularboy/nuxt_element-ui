<template>
  <div>
    one
    <button @click="dd">111</button>
    <nuxt-link to="/">index</nuxt-link>
  </div>
</template>

<script>
  import {getData} from '@/plugins/axios.js'

  export default {
    methods: {
      dd() {
        getData('1', 'put', {}).then(res => {
          console.log(res)
        }).catch(err => {
          console.log(err)
        })
      }
    }
  }
</script>

<style>

</style>
