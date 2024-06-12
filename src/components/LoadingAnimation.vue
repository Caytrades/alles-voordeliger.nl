<template>
    <div class="container">
        <div class="loader">
            <div class="center">
            </div>
            <div class="vertical"></div>
            <div class="horizontal"></div>
        </div>
        <p class="p1">
            <span class="span1">L</span>
            <span class="span2">O</span>
            <span class="span3">A</span>
            <span class="span4">D</span>
            <span class="span5">I</span>
            <span class="span6">N</span>
            <span class="span7">G</span>
        </p>
        <p class="p2">Please <strong>wait...</strong>While we are processing your request</p>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.container{
    margin: 0;
}

.loader{
    position: relative;
    height: 30vh;
    width: 30vh;
    background-color: white;
    margin: 25vh auto 0 auto;
    border: 2.5vh solid royalblue;
    border-radius: 20vh;
    animation: Loading 1s linear 0.5s infinite;
}

.center {
    position: absolute;
    height: 28vh;
    width: 28vh;
    background-color: #5555EB;
    left: 1vh;
    top: 1vh;
    border-radius: 14vh;
    z-index: 1;
  }
  
  .vertical {
    position: absolute;
    background-color: white;
    height: 35vh;
    width: 12vh;
    top: -2.5vh;
    left: 9vh;
  }
  
  .horizontal {
    position: absolute;
    background-color: white;
    height: 12vh;
    width: 35vh;
    top: 9vh;
    left: -2.5vh;
  }
  
  .p1 {
    display: block;
    position: relative;
    margin: -18.5vh auto 0 auto;
    text-align: center;
    font-size: 2.5vh;
    z-index: 1;
    color: white;
  }
  
  .span1 {
    animation: text 1s alternate 0.5s infinite;
  }
  
  .span2 {
    animation: text 1s alternate 0.7s infinite;
  }
  
  .span3 {
    animation: text 1s alternate 0.9s infinite;
  }
  
  .span4 {
    animation: text 1s alternate 1.1s infinite;
  }
  
  .span5 {
    animation: text 1s alternate 1.3s infinite;
  }
  
  .span6 {
    animation: text 1s alternate 1.5s infinite;
  }
  
  .span7 {
    animation: text 1s alternate 1.7s infinite;
  }
  
  .p2 {
    position: relative;
    text-align: center;
    font-size: 2.7vh;
    margin: 25vh auto 0 auto;
    color: #5555EB;
    font-family: Georgia;
  }
  
  @keyframes Loading {
    from {transform: rotate(0deg);}
    to {transform: rotate(360deg);}
  }
  
  @keyframes text {
    from {font-size: 2.5vh; font-weight: normal;}
    to {font-size: 3.5vh; font-weight: bold;}
  }
</style>