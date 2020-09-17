<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="blue"  app>
      <v-toolbar-title>Application</v-toolbar-title>
       <!-- Component Example -->
      <VuetifyLogo/>
       <navBar/>         
    </v-app-bar>
    v-but

    <v-spacer></v-spacer>
<v-btn icon href="/fooRoute" target="_blank">
  <v-icon>window</v-icon> Link Text
</v-btn>

   
    <!-- Body -->
    <v-content light>
      <nuxt /> 
     
    </v-content>
  
      
     
    <!-- Footer -->
   
    <v-footer color="indigo" app>
      <span class="white--text">&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
    <footer/>

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 0.5px solid;
  }

 #inspire {
    background-color: white;
    color: black;
  }
</style>