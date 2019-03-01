<template>
  <v-btn type="button" @click="goTo">Rock Stars</v-btn>
</template>

<script>

export default {
  props:{
    pathname: {
      type: String,
      required: true
    }
  },
  methods: {
    goTo() {
      this.$router.push({name: this.pathname})
    }
  }
}
</script>