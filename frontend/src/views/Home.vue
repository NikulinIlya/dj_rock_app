<template>
  <section class="container">
    <h1>Welcome to your APP</h1>
    <redirectButton pathname="rockstars"></redirectButton>
  </section>
</template>

<script>
  import redirectButton from '@/components/buttons/Redirect'

  export default {
    components: {
      redirectButton
    }
  }
</script>
