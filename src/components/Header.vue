<template>
 <header>
    <!-- <h1>{{title}}</h1> -->
    <h1>{{propTitle}}</h1> 
    <button v-on:click="changePrimitive">Change the Primitive</button>
 </header>
</template>

<script>


export default {
  name: "app",
  props:{
      propTitle:{
          type:String
      }
  },
  data() {
    return {
        title:'Archive'
    };
  },
  methods: {
    changePrimitive: function(){
      //this.propTitle="BalaBla" ; 
      console.log("inside changePrimitive");
      this.$emit('changePrimitive', 'Archive');
    }
  }
};
</script>

<style>
header{
background: lightgreen;
padding:10px;
}

h1{
    color:#222;
    text-align: center;
}

</style>
