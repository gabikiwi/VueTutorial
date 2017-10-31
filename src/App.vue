<template>
  <div>
    <app-header v-bind:propTitle="propTitle"></app-header>
    <app-content v-bind:myArray="myArray"></app-content>
    <hr>
    <app-content v-bind:myArray="myArray"></app-content>
    <app-footer v-bind:propTitle="propTitle"></app-footer>
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
        { name: "Slot1", speciality: "DescriptionSlot1", show: false},
        { name: "Slot2", speciality: "DescriptionSlot2", show: false },
        { name: "Slot3", speciality: "DescriptionSlot3", show: false }
      ],
      propTitle:"!!Another Client!!"
    };
  }
};
</script>

<style >

</style>
