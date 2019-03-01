<template>
  <v-footer
      height="auto"
      color="primary lighten-1"
      fixed
  >
    <v-layout
        justify-center
        row
        wrap
    >
      <router-link
          v-for="link in links"
          :key="link"
          :to="link"
      >
        <v-btn
            color="white"
            flat
            round>
          {{ link }}
        </v-btn>
      </router-link>
      <v-flex
          primary
          lighten-2
          py-3
          text-xs-center
          white--text
          xs12
      >
        &copy; 2019
      </v-flex>
    </v-layout>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'Home',
        'Rock Stars',
        'About Us',
      ]
    })
  }
</script>