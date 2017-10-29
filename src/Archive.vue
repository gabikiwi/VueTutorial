<template>
  <div>
    <ul>
        <li v-for="myVar in myArray">{{myVar}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
        myArray:['Ana te iubesc!', 'Magda','Gabriel']
    }
  },
  methods:{
    greeting:function(){
      return 'hey there!';
    }

  }
}
  

</script>

<style>
</style>
