<template>
    <div class="main">
        <v-card
          loading="info"
          class="mx-auto card--info"
          outlined
        >
        {{}}
        </v-card>  
    </div>    
</template>
<script lang="ts">
import Vue from 'vue';
import Component from "vue-class-component";
@Component({
    name: 'InfoOverview',
    props: {

    }
})
export default class Info extends Vue {
    constructor() {
        super();
    }
}
</script>
<style lang="scss" scoped>

</style>