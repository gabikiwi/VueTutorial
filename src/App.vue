<template>
  <div>
    <h1>{{title}}</h1>
    <p>{{greeting()}}</p>
    <archive></archive>
  </div>
</template>

<script>
import Client from './Archive.vue'

export default {
  components: {
    archive:Client
  },
  name: 'app',
  data () {
    return {
      title: 'Client Application!'
    }
  },
  methods:{
    greeting:function(){
      return 'hey there!';
    }

  }
}
  

</script>

<style scoped>
h1{
  color: blueviolet;
}
</style>
