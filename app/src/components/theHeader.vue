<template>
<div class="box">
    <h1>Header</h1>
</div>
</template>

  
<script>
export default {
    name: 'The_Header',
    props: {
        msg: String
    }
}
</script>

  <!-- Add "scoped" attribute to limit CSS to this component only -->
  
<style scoped>
.box {
    background-color: black;
    color: white;
}
</style>
