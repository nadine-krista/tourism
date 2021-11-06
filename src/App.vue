<template> 
  <router-view />
</template>

<style lang="scss">
*{
  margin:0;
  padding:0;
  outline:0;
  box-sizing: border-box;
  top:0;
  bottom:0;
  }
  body{
     min-height:100vh;
      background-size: cover;
      background-repeat: no-repeat;
      background-image: url('./assets/home/background-home-mobile.jpg');
    }
    #app{
      height:100vh;
      }
    @media only screen and (min-width:600px){
   body{
     background-image:url('./assets/home/background-home-tablet.jpg');
    }
  }
  @media only screen and (min-width:768px){
    body{
      background-image:url('./assets/home/background-home-desktop.jpg');
    }
  }

</style>
