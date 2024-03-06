<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import container from'@/views/container.vue'

import wiki from'@/views/wiki/wiki.vue'

import tabs from'@/views/tabs.vue'

</script>

<template>


  <header >
    
    <!-- <container /> -->
    <wiki /> 

  <!-- <tabs /> -->
  </header>

</template>

<style> 
	@import './font-style/font.css';
	header {
		font-family: AlibabaPuHuiTi-2-35-Light; 
    
	}
  

  *{
    font-size: x-large;
  }
</style>

