<template>
  <v-bottom-navigation
    :value="activeBtn"
    grow
    color="teal"
    width="60%"
    class="menu"
  >
    <v-btn>
      <span>Blog</span>
      <v-icon>mdi-post-outline</v-icon>
    </v-btn>

    <v-btn>
      <span>Favorites</span>
      <v-icon>mdi-heart</v-icon>
    </v-btn>

    <v-btn>
      <span>Nearby</span>
      <v-icon>mdi-map-marker</v-icon>
    </v-btn>
  </v-bottom-navigation>
</template>

<script>
export default {
  data () {
    return {
      activeBtn: 1
    }
  }
}
</script>
<style scoped>
.menu {
  margin-left: 20%;
  margin-bottom: 30px;
}
</style>
