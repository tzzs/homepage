<template>
  <v-bottom-navigation
    :value="activeBtn"
    grow
    color="teal"
    width="60%"
    class="menu"
  >

    <v-btn>
      <span>Index</span>
      <v-icon>mdi-home-outline</v-icon>
    </v-btn>

    <v-btn>
      <span>Blog</span>
      <v-icon>mdi-post-outline</v-icon>
    </v-btn>

    <v-btn>
      <span>Me</span>
      <v-icon>mdi-heart</v-icon>
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
  bottom: 20px;
  position: fixed;
}
</style>
