<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
    The Roman Empire, at its height (c. 117 CE), was the most extensive political and social structure in western civilization.
     <div class=card>
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
 </div> </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
:root{
  background-color: rgba(205, 0, 0,1);
}
.card{
    background-color: rgb(155, 63, 63);
    border:red;
    width:50%;
    margin-left: 25%;
    padding:5px;
}
h3 {
  color:plum;
  margin: 40px 0 0;
}
ul {
  
  list-style-type:lower-roman;
  padding: 0;
  color:royalblue;
}
li {
  
  display: inline-block;
  margin: 0 10px;
    

}
a {
  color:goldenrod;
}
</style>
