<template>
  <div class="home">
   <h1>home page </h1>
   <Child 
     
      @changeName ='wrrite'
      :title ='walaa' 
      age='14'
    />
   
   </div>
</template>

<script>

import Child from './Child.vue' 
export default {
  name: 'Home',
  components: {
     Child
  },
  data(){
    return {
      walaa: 'wa'
    }
  },
  methods: {
    wrrite (val){
      console.log(val);

    }
  }
 
  }

</script>
