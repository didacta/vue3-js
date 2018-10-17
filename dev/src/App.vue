
<template>
 <v-app id="app">
    <div id="nav" >
    <v-tabs color="rgb(133, 22, 22)" slider-color="red" grow>
         <v-tab :key="i" :href="`#tab-${i}`" ripple> Military </v-tab>       
          <v-tab ripple> Politics </v-tab>       
         <v-tab ripple> Economy </v-tab>       
         </v-tabs>
             </div>
    <router-view/>
       <v-footer dark absolute="true"></v-footer>
 </v-app>  
</template>

<style lang="scss">
#app {
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
  padding: 10px;
  text-align: left;
  margin-bottom: 20px;
  border-radius: 1%;
  font-family: "Quattrocento", serif;
  box-shadow: 10px 5px 18px 0px rgba(0, 0, 0, 0.75);
  background: linear-gradient(
    bottom-right,
    rgb(133, 22, 22),
    rgb(216, 37, 37),
    grey
  );
  
  .logo {
    @media only screen and (max-width: 1150px) {
      display: none;
    }
  }
  a {
    width: 180px;
    font-size: 18px;
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
