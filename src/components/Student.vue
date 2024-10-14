<template>
  <div>
   <h2>{{userName}}</h2>
   <h3>{{point}}</h3>
  </div>
</template>

<script>
export default {
name:'StudentVue',
props:{
    userName:{
        type:String,
        required:true
    },
    point:{
        type:Number,
        required:true
    }
}
}
</script>

<style>

</style>