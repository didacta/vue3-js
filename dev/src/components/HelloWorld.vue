<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
   
    <div class="cards">
      
     <div class=card>
              <img alt="Vue logo" src="../../src/assets/logo.png" class="logo">
<h2>Links</h2><hr style="height:1px;border:none;color:#333;background-color:#333;margin-bottom:20px;">
    <h3>Political Life</h3>
  
    <ul>
      <li><a href="https://en.wikipedia.org/wiki/Roman_Republic" target="_blank" rel="noopener">Early Republic</a></li>
      <li><a href="https://en.wikipedia.org/wiki/Roman_Empire" target="_blank" rel="noopener">Post Imperial  </a></li>
    </ul>
    <h3>Military</h3>
    <ul>
      <li><a href="https://romanmilitary.net/strategy/structure/" target="_blank" rel="noopener">Organization & Ranks </a></li>
      <li><a href="http://www.ancientmilitary.com/roman-weapons.htm" target="_blank" rel="noopener">Weapons</a></li>
      <li><a href="https://en.wikipedia.org/wiki/Roman_infantry_tactics" target="_blank" rel="noopener">Strategy</a></li>
      <li><a href="hhttps://en.wikipedia.org/wiki/Demography_of_the_Roman_Empire" target="_blank" rel="noopener">Demographics</a></li>
    </ul>
    <h3>Economy</h3>
    <ul>
      <li><a href="http://mariamilani.com/ancient_rome/ancient_roman_jobs.htm" target="_blank" rel="noopener">Jobs</a></li>
      <li><a href="https://www.nationalgeographic.org/media/roman-empire-road-and-trade-network/" target="_blank" rel="noopener">Trade</a></li>
      <li><a href="http://www.rsrc.ugent.be/file/24" target="_blank" rel="noopener">Resources</a></li>
      <li><a href="https://en.wikipedia.org/wiki/Slavery_in_ancient_Rome" target="_blank" rel="noopener">Slavery</a></li>
    </ul>
 </div>
  <div class=bigcard>  <code>
    The Roman Empire, at its height (c. 117 CE), was the most extensive political and social structure in western civilization.</code>
    <img alt="Roman Empire 117 A.D" src="https://imgur.com/QuuD7w1.png" class="map">
    </div> 
 <div class=card>       <img alt="Vue logo" src="../../src/assets/logo.png" class="logo"> 
 <h2>News</h2><hr style="height:1px;border:none;color:#333;background-color:#333;margin-bottom:20px;">

 <v-alert :value="true" type="warning" outline="true" dismissible="true">Constantinople has fallen. </v-alert>
  <v-alert :value="true" type="error" outline="true" dismissible="true">Barbarians are attacking!</v-alert>
    <v-alert :value="true" type="success" color="#CE8E8E" dismissible="true">You have repaired the city walls.</v-alert>


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
background-image: url('http://666a658c624a3c03a6b2-25cda059d975d2f318c03e90bcf17c40.r92.cf1.rackcdn.com/unsplash_527bf56961712_1.JPG');
}
code{
  background-color:rgb(0, 0, 0);
  color:rgb(80, 8, 14);
}
v-alert{
    font-family: "Quattrocento", serif;

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
  box-shadow: 4px 2px 18px 0px rgba(0, 0, 0, 0.75);
  @media only screen and (max-width: 1250px) {
    display: none;
  }
}
.card {
  flex: 0 1 22%;
  background-color: rgb(133, 22, 22);
  border-radius: 2%;
  margin: 15px;
  padding: 10px;
  box-shadow: 4px 2px 18px 0px rgba(0, 0, 0, 0.75);
  @media only screen and (max-width: 1250px) {
    flex: 0 1 44%;
  }
  @media only screen and (max-width: 850px) {
    flex: 0 1 200%;
  }
}
.map{
  height:400px;
  width:573.5px;
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
h1,h2,h3 {
  font-family: "Quattrocento", serif;
}
h3 {
  color: plum;
  margin: 20px 0 0;
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
  font-size: 18px;
}
hr {
  color:red;
}
ol {
  list-style-type: upper-roman;
}
</style>
