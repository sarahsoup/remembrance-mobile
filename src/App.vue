<template>
  <div id="app">
    <!-- <div class="background-image">
      </div> -->
      <div class="app-content"
    <router-view/>
  </div>
  </div>

</template>

<script>
export default {
  name: 'app',
  methods: {
    track () {
      this.$ga.page('/')
    }
  },
  created () {
            document.title = "Remembrance Climate Futures"
            
        }
}

</script>

<style>

body{
  height: 100%;
}

@font-face{
  font-family: 'PlayfairSC';
  src: url('assets/fonts/PlayfairDisplaySC-Regular.ttf') format('truetype');
}

@font-face{
  font-family: 'CaslonSC';
  src: url('assets/fonts/caslon.otf') format('opentype');
}

@font-face{
  font-family: 'Trade';
  src: url('assets/fonts/trade.ttf') format('truetype');
  font-weight: normal;
}

@font-face{
  font-family: 'Trade';
  src: url('assets/fonts/trade-condensed.ttf') format('truetype');
  font-weight: bold;
}

html{
  /* height: 100%; */
  
  /* height: 100vh; */
  /* width: 400px; */
  /* background-position: center; */
  /* background-repeat: no-repeat; */
  /* background-size: 100vh; */
  /* position: relative; */
  /* background-position: right; */
  /* transform: rotate(20deg); */
  /* -webkit-filter: blur(5px);  */
  /* Safari 6.0 - 9.0 */
    /* filter: blur(5px); */
}

#app {
  font-family: 'PlayfairSC', 'Trade', Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  height: 100%;
  /* color: #2c3e50; */
  
  scroll-snap-destination: 0vw 0vh;
  -webkit-scroll-snap-type: proximity;
  -ms-scroll-snap-type: proximity;
  scroll-snap-type: proximity;
  scroll-behavior: smooth;
  /* overflow-x: hidden; */
  overflow-y: auto;
  /* z-index: -9999; */

}

.background-image{
  position: fixed;
  left: 0;
  right: 0;
  height: 100vh;
  /* width: 100vw; */
  color: rgb(0, 0, 0); 
  background-attachment: fixed;
  /* background-size:50%; */
  background-repeat: no-repeat;
  -webkit-filter: blur(5px); /* Safari 6.0 - 9.0 */
    filter: blur(5px);
    z-index: -999999;

}
.app-content{

  position: fixed;
  left: 0;
  right: 0;
  z-index: 9999;

}

.about-s {
  ont-family: 'CaslonSC';
  color: #fff;
  font-weight: normal;
  text-transform: lowercase;
  font-size: 18px !important;
}
#app h1{
  font-family: 'CaslonSC';
  color: #fff;
  font-weight: normal;
}

#app h2{
  font-family: 'CaslonSC';
  color: #fff;
  font-weight: normal;
}

#app h3{
  font-family: 'Trade';
  color: #000;
}

#app p{
  font-family: 'Trade';
  color: #fff;
}

#app a {
  color: #fff;
  text-decoration: underline;
}

#app .label-text{
  font-size: 10px;
  font-family: 'Trade';
  color: #000;
}

.home {
  /* overflow: hidden; */
  /* z-index: 9999; */
}


.splash-txt{
  position: absolute;
  top: 50%;
  left: 60px;
  color: white;
}

.splash-txt h3{
  font-size: 40px;
  line-height: 1;
  letter-spacing: 1.6px;
}

.intro{
  padding: 40px 20px 80px 60px;
}

#icon-div{
  position: fixed;
  top: 10px;
  right: 10px;
}
.icon-div{
  position: fixed;
  top: 10px;
  right: 10px;
}

.splash-img { 
  position: fixed; 
  /* width: 15%; */
  /* height: auto;  */
  width: auto;
  height: 500px;
  /* width: 400px; */
  top: .18vh;
  left: -50vw;
  z-index: -1999;
  opacity: 0.8;
  -webkit-filter: blur(.1px); /* Safari 6.0 - 9.0 */
  filter: blur(.1px);
  filter: brightness(75%);
  
  
  
}


svg {
  position: fixed; 
  height: 100vh;
  width: 100vw;
}

.backgear-cr {
  fill: #333;
  opacity: .25;
}

.backgear-img { 
  position: fixed; 
  /* width: 15%; */
  /* height: auto;  */
  width: auto;
  height: 260vh;
  opacity: .85;
  /* width: 400px; */
  top: .18vh;
  left: -50vw;
  z-index: -5999;
  /*filter: sepia(10%) saturate(100%) brightness(10%) ;*/
  -webkit-filter: blur(4px); /* Safari 6.0 - 9.0 */
    filter: blur(4px);
}

  #extra-icon, #about-button{
    font-family: Trade;
    font-weight: bold;
    padding: 0.5em;
    padding-top: 0.6em;
    //color: white;
    border-radius: 2px;
    border: none;
    box-shadow: none!important;
    background-color: rgba(0, 0, 0, 0.1);

  }

#extra-icon:hover, #about-button:hover{
  background-color: rgba(255, 255, 255, 0.5);

}
  #extra-content{
    /*column-count: 2;
    column-gap: 0;
    background-color: rgba(0, 0, 0, 0.5);*/
  }


 


</style>
