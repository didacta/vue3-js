
<template>
 <v-app id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
     <v-btn color="error">   <router-link to="/pol">Politics</router-link></v-btn>
     <v-btn color="error"><router-link to="/econ">EconomyE</router-link></v-btn>
    <v-btn color="error"><router-link to="/mil">Military</router-link></v-btn>
      
    
      
    </div>
   
    <router-view/>

      </v-app>
</template>


<style lang="scss">
//shapes
$triangle: polygon(100% 0, 0% 100%, 100% 100%);
$cirlce:50%;

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:gold;
  background:linear-gradient(to top,red, whitesmoke);
}
#nav {
  padding: 20px;
  text-align: left;
  a {
    
    padding-right: 5px;
    font-size: 20px;
    font-weight: bold;
    color:palevioletred;
    &.router-link-exact-active {
      color:darkred;
    }
  }
}
</style>
