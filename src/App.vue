<template>
  <div>
    <h1>Implementing two way data binding without using V-Model -:</h1>
    <input type="text" :value="myinput" @input="changing"/>
    <h2>{{myinput}}</h2>
  </div>
</template>

<script>
export default {
  data:function(){
      return{
        myinput : "write here"
      }
  },
  methods:{
    changing(e){
      console.log("hi");
      this.myinput = e.target.value;
    }
  }
}
</script>

<style scoped>

</style>