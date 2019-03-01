<template>
  <v-layout class="pa-3">
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-img
          :src="require('../assets/img/steven_tyler.jpg')"
          contain
        >
        </v-img>
        <v-container fill-height fluid>
          <v-layout fill-height>
            <v-flex xs12 align-end flexbox>
              <span class="headline">Steven Tyler</span>
            </v-flex>
          </v-layout>
        </v-container>
        <v-card-title>
          <div>
            <span class="grey--text">Aerosmith</span><br>
            <span>Singer</span><br>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>

    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-img
          :src="require('../assets/img/freddie_mercury.jpg')"
          contain
        >
        </v-img>
        <v-container fill-height fluid>
          <v-layout fill-height>
            <v-flex xs12 align-end flexbox>
              <span class="headline">Freddie Mercury</span>
            </v-flex>
          </v-layout>
        </v-container>
        <v-card-title>
          <div>
            <span class="grey--text">Queen</span><br>
            <span>Singer</span><br>
          </div>
        </v-card-title>
        <v-card-actions>
          <v-btn flat color="orange">Share</v-btn>
          <v-btn flat color="orange">Explore</v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
  export default {
    data () {
      return {
      }
    }
  }
</script>