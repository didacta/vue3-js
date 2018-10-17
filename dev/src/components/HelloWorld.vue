<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
   
    <div class="cards">
      
     <div class=card>
              <img alt="Vue logo" src="../../src/assets/logo.png" class="logo">

    <h3>Political Life</h3>
  
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">Early Republic</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">Post Imperial  </a></li>
    </ul>
    <h3>Military</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Organization & Ranks </a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Weapons</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Strategy</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Demographics</a></li>
    </ul>
    <h3>Economy</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">Jobs</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">Trade</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">Banking</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">Resources</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">Slavery</a></li>
    </ul>
 </div>
  <div class=bigcard>  <code>
    The Roman Empire, at its height (c. 117 CE), was the most extensive political and social structure in western civilization.</code></div> 
 <div class=card>       <img alt="Vue logo" src="../../src/assets/logo.png" class="logo"> 
 <v-alert :value="true" type="warning" outline="true" dismissible="true">Constantinople has fallen </v-alert>
  <v-alert :value="true" type="error" outline="true" dismissible="true">The Turks are attacking!</v-alert>
    <v-alert :value="true" type="success" color="#CE8E8E" dismissible="true">You have repaired the city walls</v-alert>


 </div>
 

    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
:root {
  background-color: rgba(205, 0, 0, 1);
}
.cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.bigcard {
  flex: 0 1 42%;
  background-color: rgb(133, 22, 22);
  width: 50%;
  border-radius: 2%;
  margin: 15px;
  padding: 15px;
  box-shadow: 10px 5px 18px 0px rgba(0, 0, 0, 0.75);
  @media only screen and (max-width: 1150px) {
    display: none;
  }
}
.card {
  flex: 0 1 22%;
  background-color: rgb(133, 22, 22);
  border-radius: 2%;
  margin: 25px;
  padding: 10px;
  box-shadow: 10px 5px 18px 0px rgba(0, 0, 0, 0.75);
  @media only screen and (max-width: 1150px) {
    flex: 0 1 44%;
  }
  @media only screen and (max-width: 850px) {
    flex: 0 1 200%;
  }
}

.logo {
  top: 50%;
  left: 50%;
  margin-top: -45px;
  margin-left: -5px;
  height: 160px;
  width: 160px;
  @media only screen and (max-width: 1150px) {
    display: none;
  }
}
h1 {
  font-family: "Quattrocento", serif;
}
h3 {
  color: plum;
  margin: 40px 0 0;
}
ul {
  padding: 0;
  color: royalblue;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: goldenrod;
}
ol {
  list-style-type: upper-roman;
}
</style>
