<template>
    <div id="header">
        <img class="logo-header" :src="image"/>
        <hr/>
        <nav role="navigation" class="main-nav">
            <ul>
                <li>00 <span>Home</span></li>
                <li>01 <span>Destination</span></li>
                <li>02 <span>Crew</span></li>
                <li>03 <span>Technology</span></li>
            </ul>
        </nav>
    </div>
</template>
<script>
import image from "../assets/shared/logo.svg";
export default{
    name:"Header",
    data(){
        return {image};
    }
}
</script>
<style>
#header{
   
   display: grid;
   gap:20px;
   height:96px;
   
   align-items: center;
   grid-template-areas: 
   "logo",
   "nav";
}
hr{
    margin-left:44px;background: #FFFFFF;
mix-blend-mode: normal;
opacity: 0.25;
margin-right:-60px;
position:relative;
z-index:9999999;
}

nav ul{
    display: flex;
    justify-content: space-around;
    list-style-type: none;
    align-items: center;
    padding:0px 123px;
    height:inherit;
}

nav ul li{
    color:#fff;
    font-family: 'Barlow Condensed';
    font-style: normal;
    font-weight: bold;
    font-size: 16px;
    line-height: 19px;
    letter-spacing: 2.7px;
    display:flex;
    height:inherit;
    align-items: center;
    border-bottom:2px solid #FFF;
}
nav ul li span{
    font-weight: normal;
    margin-left:5px;
    text-transform: uppercase;
}
.logo-header{
    margin-left:55px;
    grid-area:logo;
    width:48px;
    height:48px;
}
.main-nav{
    grid-area:nav;
    background: rgba(255, 255, 255, 0.04);
    backdrop-filter: blur(81.5485px);
    height: inherit;
}
@media only screen and (min-width:600px){
   #header{
     grid-template-columns: 1fr 1fr 3fr;
     grid-template-areas: 
     "logo . nav";
   }
}
@media only screen and (min-width:768px){
     #header{
     grid-template-columns: 0.5fr 2fr 4fr;
     grid-template-areas: 
     "logo . nav";
   }
}
</style>