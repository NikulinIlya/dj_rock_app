<template>
  <v-toolbar dark color="primary">
    <v-toolbar-side-icon></v-toolbar-side-icon>

    <v-toolbar-title class="white--text">Title</v-toolbar-title>

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
        'Home',
        'Rock Stars',
        'About Us',
      ]
    })
  }
</script>