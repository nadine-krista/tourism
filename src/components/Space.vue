<template>
    <div id="space-travel">
        <div class="title">
SO, YOU WANT TO TRAVEL TO
        </div>
        <div class="space">
            SPACE
        </div>
        <div class="face-it">
            Let’s face it; if you want to go to space, you might as well genuinely go to outer space and not hover kind of on the edge of it. Well sit back, and relax because we’ll give you a truly out of this world experience!
        </div>
    </div>
</template>
<script>

export default{
    name:"Space",  
}
</script>
<style>
#space-travel{
  width: 450px;
 
  display: flex;
  flex-direction: column;
}
.title{
    font-family: 'Barlow Condensed';
    font-style: normal;
    font-weight: normal;
    font-size: 28px;
    line-height: 34px;
    /* identical to box height */
    letter-spacing: 4.725px;
    color: #D0D6F9;
}
.space{
    font-family: 'Bellefair';
    font-style: normal;
    font-weight: normal;
    font-size: 150px;
    line-height: 172px;
    /* identical to box height */
    color: #FFFFFF;
}
.face-it{
    font-family: 'Barlow';
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 32px;
    /* or 178% */
    color: #D0D6F9;
}
@media only screen and (min-width:600px){
   
}
@media only screen and (min-width:768px){
 
}
</style>