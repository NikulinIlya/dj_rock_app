<template>
  <v-footer
      height="auto"
      color="primary lighten-1"
  >
    <v-layout
        justify-center
        row
        wrap
    >
      <router-link
          v-for="link in links"
          :key="link"
          :to="link.path"
      >
        <v-btn
            color="white"
            flat
            round>
          {{ link.name }}
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
        {'path': '/',
        'name': 'Home'},
        {'path': 'rockstars',
        'name': 'Rock Stars'},
        {'path': 'about',
        'name': 'About Us'}
      ]
    })
  }
</script>