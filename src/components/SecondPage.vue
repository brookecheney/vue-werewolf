<template>
  <v-app id="inspire">

   
    
    <!-- <v-navigation-drawer
      class="top"
      v-model="drawer"
      app
      clipped
    >
      <v-list dense>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-view-dashboard</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Dashboard</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link>
          <v-list-item-action>
            <v-icon>mdi-settings</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Settings</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->

 
    

    <v-content>
     
      <v-container
        class="fill-height"
        fluid
      >
   
        <v-row
          align="center"
          justify="center"
        >
          <v-col class="shrink">
            
                   <div class="text-center">
  <h1>WereWolf</h1>
  <br>
  <br>
  <br>

  <br>
  <p> Are you a moderator or player?</p>
  <br>
<div>
<router-link to="/SecondPage" class="none">
    <v-btn fab x-large rounded color="#AA5F2C" dark class="start" id="start" v-on:click="method">
      Player</v-btn></router-link> 
</div>
<br>
<br>
<div>
      <router-link to="/EnterPlayer" class="none">
    <v-btn fab x-large rounded color="#AA5F2C" dark class="start" id="start" v-on:click="method">
      Moderator</v-btn></router-link> 
      </div>
  </div>
       
          </v-col>
      
        </v-row>
      </v-container>
    </v-content>

   
</v-app>
</template>
<style scoped>

h1 {
  letter-spacing: 2px;

}
p {
  color: white;
  letter-spacing: 1px;
  font-size:20px;
}
</style>
<script>
  export default {
    name: 'SecondPage',


    data: () => ({
      title: 'This is the second page'
    }),
  }
</script>