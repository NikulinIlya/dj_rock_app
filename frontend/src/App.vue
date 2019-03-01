<template>
  <v-app id="app">
    <MyHeader></MyHeader>
    <h1> Some content... </h1>
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