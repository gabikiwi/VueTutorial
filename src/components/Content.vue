<template>
<div id="myArray">
    <ul>
    <li v-for="myVar in myArray" v-on:click="myVar.show=!myVar.show">
        <h2>{{myVar.name}}</h2>
        <h3 v-show="myVar.show">{{myVar.speciality}}</h3>
    </li>
    </ul>
    <button v-on:click="deleteArrayElement">Delete an Reference</button>
</div>
</template>

<script>
export default {
  props: {
      myArray:{
          type:Array,
          required:true
      }
  },
  data() {
    return {};
  },
  methods: {
    deleteArrayElement: function(){
      this.myArray.pop(); 
    }
  }
};
</script>

<style scoped>
#myArray {
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
}
</style>
