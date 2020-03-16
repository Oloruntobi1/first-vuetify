<template>
  <v-app>
    <!-- <v-app-bar app color="primary" dark>
      <v-toolbar-title>Vuetify Dashboard</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text rounded to="/">Home</v-btn>
      <v-btn text rounded to="/login">Login</v-btn>
      <v-btn 
        v-for="link in links"
        :key="`${link.label}-header-link`"
        text 
        rounded 
        :to="link.url"
      >
      {{ link.label }}
      </v-btn>
    </v-app-bar> -->
    <navbarlink></navbarlink>
    <v-content>
      <router-view></router-view>
    </v-content>
    <!-- <v-footer color="primary lighten-1" padless>
      <v-layout justify-center wrap>
        <v-btn
          v-for="link in links"
          :key="link"
          color="white"
          text
          rounded
          class="my-2"
        >
          {{ link }}
        </v-btn>
        <v-btn
          v-for="link in links"
          :key="`${link.label}-footer-link`"
          color="white"
          text
          rounded
          class="my-2"
          :to="link.url"
        >
          {{ link.label }}
        </v-btn>
        <v-flex primary lighten-2 py-4 text-center white--text xs12>
          {{ new Date().getFullYear() }} — <strong>Vuetify Dashboard</strong>
        </v-flex>
      </v-layout>
    </v-footer> -->

    <footerlink></footerlink>
  </v-app>
</template>

<script>
import navbarlink from '@/components/navbarlink.vue'
import footerlink from '@/components/footerlink.vue'

export default {
  name: 'App',
  components: {
    navbarlink,
    footerlink
  },
  
}
</script>