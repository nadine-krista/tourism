<template>
<div id="main-container">
  <header>
    <Header/>
  </header>
  <main>
    <Space/>
    <Explore/>
  </main>
</div>
  
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Header from "../components/Header.vue";
import Explore from "../components/Explore.vue";
import Space from '../components/Space.vue';

@Options({
  components: {
    Header,
    Explore,
    Space
  },
})
export default class Home extends Vue {}
</script>
<style>
*{
  margin:0;
  padding:0;
  outline:0;
  box-sizing: border-box;
  }
header{
  padding-top:40px;
  
}

main{
 display:flex;
 flex-direction: row;
  bottom:131px;
  padding:0px 165px 60px;;
  justify-content: space-between;
  align-items: flex-end;
  flex-grow: 1;
  
}
#main-container{
  height: 100vh;
  display: flex;
  flex-direction: column;
 
}

  @media only screen and (min-width:1440px){
    #main-container{
     width:1440px;
    }
  }
</style>
