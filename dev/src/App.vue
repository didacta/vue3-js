
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
<div id="footer">
 <v-footer
    dark
    height="80px" 
    color=#7C0A02
    
  >
    <v-card
      flat
      tile
      color=#7C0A02
      height="80px"
    >
      <v-card-text absolute=true>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-3 white--text"
          icon
        >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-btn>
         <v-card-text class="white--text pt-0">        
      </v-card-text>

      </v-card-text>

     
      <v-divider></v-divider>

    </v-card>   
        &copy;2018 — <strong>Igor Yermak</strong> 
  </v-footer>
</div>
 </v-app>  
 
</template>

<script>
export default {
  data: () => ({
    icons: [
      "fab fa-twitter",
      "fab fa-linkedin",
      "fab fa-instagram",
      "far fa-envelope"
    ]
  })
};
</script>

<style lang="scss">
#app {
  background-image: url("https://c1.staticflickr.com/3/2122/2367097282_8e81c2134d_o.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-color: rgba(200, 100, 0, 0.5); // Tint color
  background-blend-mode: multiply;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: gold;
  font-family: "Quattrocento-Bold", serif;
}
#nav {
  display: flex;
  flex-wrap: wrap;
  padding: 0.2px;
  text-align: left;
  margin-bottom: 15px;
  font-family: "Quattrocento", serif;
  box-shadow: 6px 2px 18px 0px rgba(0, 0, 0, 0.75);
  background-color: transparent;
  opacity: 0.6;

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
      width: 140px;
      font-size: 16px;
    }
  }
}

#footer {
  position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
    opacity:.6; 
}
</style>
