<template>
  <div>
    <app-header></app-header>
    <app-content v-bind:myArray="myArray"></app-content>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    "app-header": Header,
    "app-content": Content,
    "app-footer": Footer
  },
  name: "app",
  data() {
    return {
      myArray: [
        { name: "Gabriel",speciality: "Senior technology Consultant", show: false},
        { name: "Ana Maria", speciality: "copil si elev", show: false },
        { name: "Magda", speciality: "Asistent SAP", show: false }
      ]
    };
  }
};
</script>

<style >

</style>
