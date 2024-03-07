<template>
  <div id="app">
      
    <div class="card-body p-2">
      <NavComp/>
      <BlueComp/>
      <HelloWorld/>
    </div>
  </div>
  
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import NavComp from './components/NavComp.vue';
import BlueComp from './components/BlueComp.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,NavComp,BlueComp
  }
}
</script>

<style>

  
</style>
