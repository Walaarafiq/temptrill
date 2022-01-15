<template>
  <div>
    <h3>child component  {{title}} {{age}} </h3>
    <input type="text" v-model="myName">
   <button @click="$emit('changeName',myName)" >click</button>
  </div>
</template>

<script>
export default {
    name:'Child',
    props: ['title','age'],
    data (){
        return {
            myName : ''
        }
    }
}
</script>

<style>

</style>
