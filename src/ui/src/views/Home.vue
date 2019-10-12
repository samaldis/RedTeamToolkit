<template>
  <main>
    <div class="home">
      <div class="col">
        <InfoOverview />
      </div>
      <div class="col">
        <div class="tools"></div>
      </div>
      <div class="col">
        <div class="term"></div>
      </div>
    </div>
  </main>
</template>

<script lang="ts">
import Vue from 'vue';
import InfoOverview from '../components/Info.vue';
export default Vue.extend({
  components: {
    InfoOverview
  },
});
</script>
<style lang="scss" scoped>
main {
  width: 100pc;
  height: 100pc;
  position: fixed;
  top:0px;
  left: 0px;
  overflow-x: hidden;
  overflow-y: scroll;
  div.col {
    width: 100pc;
    height: 40pc;
    margin: 0;
    padding: 0;
    left: 0;
    right: 0;
    overflow: hidden;
    &:nth-child(1) {
      margin-top: 55px;
    }
  }
}
.card--info {
  min-height: 20pc;
}
</style>
