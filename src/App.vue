<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
      <HelloWorld/>
    </v-content>

<!--    <v-bottom-navigation-->
<!--      :value="activeBtn"-->
<!--      grow-->
<!--      color="teal"-->
<!--      class="bottom-menu"-->
<!--      width="60%"-->
<!--    >-->
<!--      <v-btn>-->
<!--        <span>Blog</span>-->
<!--        <v-icon>mdi-post-outline</v-icon>-->
<!--      </v-btn>-->

<!--      <v-btn>-->
<!--        <span>Favorites</span>-->
<!--        <v-icon>mdi-heart</v-icon>-->
<!--      </v-btn>-->

<!--      <v-btn>-->
<!--        <span>Nearby</span>-->
<!--        <v-icon>mdi-map-marker</v-icon>-->
<!--      </v-btn>-->
<!--    </v-bottom-navigation>-->
    <TMenu></TMenu>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import TMenu from './components/TMenu'

export default {
  name: 'App',

  components: {
    HelloWorld,
    TMenu
  },

  data: () => ({
    //
    activeBtn: 1
  })
}
</script>

<style scoped>
.bottom-menu {
  margin-bottom: 30px;
  margin-left: 20%;
}
</style>
