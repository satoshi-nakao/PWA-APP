<template>
  <v-app>
    <!-- <v-navigation-drawer app v-model="drawer" clipped>Navigation Lists</v-navigation-drawer> -->
    <v-app-bar color="dark"  app clipped-left> 
      <!-- <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon> -->
      <v-btn :to="'/'">TOP</v-btn>
      <v-toolbar-title>My Page</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
      <!-- <v-btn  v-for="item in items" :key="item"  :to="item.to">{{ item.name }}</v-btn> -->
      <v-tabs>
        <v-tab v-for="item in items" :key="item" :to="item.to" >{{ item.name }}</v-tab>
      </v-tabs>
      </v-toolbar-items>
    </v-app-bar>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer  dark app>
    <v-layout justify-center>
      <span>&copy; 2021 Satohsi Nakao. All Rights Reserved.</span>
    </v-layout>
    </v-footer>
  </v-app>
</template>zz

<script>
export default {
  data(){
    return{
      drawer: false,
      items: [
        {name: 'Profile',to: '/profile'},
        {name: 'Skill',to: '/skill'},
        {name: 'Want',to: '/want'},
        {name: 'Works', to: '/works'}
      ],
    }
  }
}
</script>