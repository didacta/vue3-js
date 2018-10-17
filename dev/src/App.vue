
<template>
 <v-app id="app">
    <div id="nav" >
    <v-tabs color="black" slider-color="red" grow>
         <v-tab :key="i" :href="`#tab-${i}`" ripple> Home </v-tab>       
          <v-tab ripple> Maps </v-tab>       
         <v-tab ripple> Literature </v-tab>       
         </v-tabs>
             </div>
    <router-view/>
       <v-footer dark absolute="true">  ©Igor Yermak <br>- Pax Romana </v-footer>
 </v-app>  
</template>

<style lang="scss">

#app {
  background-image: url('http://people.ucalgary.ca/~vandersp/Courses/maps/fullmap3.jpg');
   background-color: rgba(200,100,0,.5); // Tint color
  background-blend-mode: multiply;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: rgb(148, 13, 13);
  color: gold;
  font-family: "Quattrocento-Bold", serif;
}
#nav {
  display: flex;
  flex-wrap: wrap;
  padding: .2px;
  text-align: left;
  margin-bottom: 15px;
  font-family: "Quattrocento", serif;
  box-shadow: 6px 2px 18px 0px rgba(0, 0, 0, 0.75);
  background-color: transparent;
  
  .logo {
    @media only screen and (max-width: 1150px) {
      display: none;
    }
  }
  a {
    width: 180px;
    font-size: 19px;
    font-weight: bold;
    color: goldenrod;
    &.router-link-exact-active {
      color: gold;
    }
    @media only screen and (max-width: 1150px) {
      width: 100px;
    }
  }
}
</style>
