<template>
  <footer>
    <p>{{copyright}} {{propTitle}}</p>
  </footer>
</template>

<script>
export default {
  props:{
      propTitle:{
          type:String
      }
  },
  data() {
    return {
    copyright:'Copyright 2017 Seers CX'

    };
  }
};
</script>

<style scoped>
footer {
    background: #222;
    padding:6px;
}
p{
    color:lightgreen;
    text-align: center;
}
</style>
