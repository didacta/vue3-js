
<template>
 <v-app id="app">
    <div id="nav" >
       <img alt="Vue logo" src="../src/assets/logo.png" class="logo">
     <v-btn color="pink" > <router-link to="/">Home</router-link></v-btn>
     <v-btn color="pink">   <router-link to="/pol">Politics</router-link></v-btn>
     <v-btn color="pink"><router-link to="/econ">Economy</router-link></v-btn>
    <v-btn color="pink"><router-link to="/mil">Military</router-link></v-btn>
        <img alt="Vue logo" src="../src/assets/logo.png" class="logo">
    
      
    </div>
   
    <router-view/>

      </v-app>
</template>


<style lang="scss">
//shapes
$triangle: polygon(100% 0, 0% 100%, 100% 100%);
$circle: 50%;

#app {
  $triangle:$triangle;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: rgb(148, 13, 13);
  color: gold;
}
#nav {
  display: flex;
  flex-wrap: wrap;
  padding: 10px;
  text-align: left;
  box-shadow: 10px 5px 18px 0px rgba(0, 0, 0, 0.75);
  background: linear-gradient(
    to bottom-right,
    rgb(133, 22, 22),
    rgb(216, 37, 37),
    grey
  );
  margin-bottom: 20px;
  border-radius: 1%;
  font-family: "Times New Roman", Times, serif;
  .logo {
    display: inherit;
      flex-wrap: nowrap;

    height: 145px;
    width: 105px;
    vertical-align: middle;
    margin-right: 2px;
    @media only screen and (max-width: 1150px) {
      display:none;
    }
  }
  a {
    width:180px;
    font-size: 18px;
    font-weight: bold;
    color: goldenrod;
    &.router-link-exact-active {
      color: gold;
    }
    @media only screen and (max-width: 1150px) {
      width:100px;
    }
  }
}
</style>
