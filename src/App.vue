<template>
  <div>
    <v-app>
      <app-v-toolbar></app-v-toolbar>
      <v-spacer></v-spacer>
      
      <v-spacer></v-spacer>
    </v-app>
  </div>
</template>

<script>

import ToolbarPage from './components/PageInicial/ToolbarPage.vue';

  export default {
    components: {
    'app-v-toolbar': ToolbarPage,  
  },
  }
</script>
  
<style>
  
</style>