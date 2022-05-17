<template>
  <v-app id="inspire">

    <v-app-bar
      app
      color="#primary"
      dark
      prominent
      src="https://i.postimg.cc/tRtvvqfx/To-Do-List-Logo-for-Facebook.webp"
    >
     
      <!-- <v-app-bar-title> Vuetify Todo</v-app-bar-title> -->

      <v-spacer></v-spacer>

    </v-app-bar>


    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      drawer: null,
      items: [
          { title: 'Todo', icon: 'mdi-format-list-checks', to:'/' },
          { title: 'About', icon: 'mdi-help-box', to:'/about' },
        ],
    }),
  }
</script>

<style scoped>

</style>