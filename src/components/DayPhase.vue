 <template>
  <v-app id="day">


<v-content>
<div class="text-center"><h2>Day Phase</h2></div>
     
<div class="team">
<v-container class="my-3">

<v-layout row wrap>

<v-flex xs6 sm4 md4 lg3 v-for="person in team" :key="person.name">

<v-card flat class="text-xs-center ma-4" id="border">
   <v-responsive class="pt-2">
      <div class="text-center">
      <img src="./villa.png" class="cen">
      </div>

</v-responsive> 
 

<v-card-text>
    <div class="subheading"><div class="text-center">{{ person.name }}</div></div>
    <div class="gray--text"><div class="text-center">{{ person.role }}</div></div>
</v-card-text>    
<v-card-actions>


</v-card-actions>
</v-card>
</v-flex>
</v-layout>
</v-container>
<router-link to="/DayPhase" class="next"><p>Next Step</p></router-link> 

</div>
    
       
        
    </v-content>

   
</v-app>
</template>
<style>
.next {
  padding-top:12px;
 font-size: 7px;
 
}
#border {
  border-radius: 13px;
  background-color:white;

}
.gray--text {
  color: gray;
  letter-spacing: 1px;
  font-size:20px;
  font-weight: 900px;

}
.subheading {
  color: gray;
}


p {
  color: white;
  letter-spacing: 1px;
  font-size:12px;
  font-weight: 600px;
  float: left;
}
#day {
    background-image: url('day4.png');
  background-size: cover;
   background-color: #323C46;

  background-position: bottom;
  transition: 0.4s;

   background-color: #323C46;


}
#app {
    background-image: url('/img/night.jpg');
  background-size: cover;
   background-color: #323C46;

  background-position: bottom;
  transition: 0.4s;

}
.none {
  text-decoration: none;
}
h2 {
    color: white;
    font-size: 30px;
       text-shadow: 2px 2px #595858;
   
}


h1 {

  font-style: normal;
  font-weight: 700;
  color:white;

  
  font-size: 45px;
}
header.v-sheet.v-sheet--tile.theme--dark.v-toolbar.v-app-bar.v-app-bar--fixed {
   color: white;
}
#app {
  color: orange;
}
.v-application.v-application--is-ltr.theme--dark {
  color: orange;

}
.theme--dark.v-application {
  color: orange;
}



#start {
  padding-left: 200px;
   padding-right: 200px;
   border-radius: 40px;
   font-size: 20px;
}




.start {
  padding-left: 200px;
   padding-right: 200px;
   border-radius: 40px;
   font-size: 20px;
}
.v-toolbar_content {
  color: white;
}
.v-button_content{
  color: white;
}
.v-content_wrap{
  background-color: white;
}
header {
   color: orange;
}
.v-app-bar--fixed {
   color: white;
}
.top {
 color: orange;

}
</style>
<script>
export default {
data() {
    return {
        team: [
            { name:'Brooklyne', role: 'WereWolf' },
            { name:'Court', role: 'Villager' },
            { name:'Sam', role: 'WereWolf' },
            { name:'Rudy', role: 'Doctor' },
            { name:'Randy', role: 'Villager' },

        ]

    }
}
  
};
</script>
