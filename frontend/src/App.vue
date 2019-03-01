<template>
  <v-app id="app">
    <MyHeader></MyHeader>
    <router-view></router-view>
    <MyFooter></MyFooter>
  </v-app>
</template>

<script>
import MyHeader from '@/components/Header'
import MyFooter from '@/components/Footer'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyFooter
  },
  data () {
    return {
      //
    }
  }
}
</script>

<style scoped lang="sass">
html, body
  margin: 0
  min-height: 100vh
</style>