<template>
  <v-toolbar dark color="primary">
    <v-toolbar-side-icon></v-toolbar-side-icon>

    <v-toolbar-title class="white--text">Title</v-toolbar-title>
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

    <v-spacer></v-spacer>

    <v-btn icon>
      <v-icon>search</v-icon>
    </v-btn>
  </v-toolbar>
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