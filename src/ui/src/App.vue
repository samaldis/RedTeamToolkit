<template>
  <v-app>
    <NavBar :buttons="buttons"/>
    <v-content>
      <router-view>
      </router-view>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import NavBar from './components/Nav.vue';

export default Vue.extend({
  name: 'App',
  components: {
    NavBar,
  },
  data: () => ({
     buttons : [
    {
      title: "home",
      link: "/",
    },
    {
      title: "tools",
      link: "/tools",
    },
    {
      title: "results",
      link: "/res",
    },
  ],
  }),
});
</script>
