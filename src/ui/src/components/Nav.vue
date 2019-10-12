<template>
<nav>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span></span>
        <span class="font-weight-light">RED TEAM TOOLKIT</span>
      </v-toolbar-title>
      <div class="button" v-for="button in buttons" :key="button">
          <v-spacer></v-spacer>
          <router-link :to="button.link">
                <v-btn
                    text
                    target="_blank"
                >
            <span class="mr-2">{{button.title}}</span>
          </v-btn>
        </router-link>
      </div>
      
    </v-app-bar>
</nav>
</template>

<script lang="ts">
import Vue from 'vue';
import Component from 'vue-class-component';
@Component(
    {
        props: {
            buttons: Object,
        },
        data: {
            buttons: [],
        },
    }
)
export default class NavBar extends Vue {
    constructor() {
        super();
    }
}
</script>