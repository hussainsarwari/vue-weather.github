<template>
  <div id="dashbord">
<input type="text" name="search" id="search" placeholder="Search">
<h4>Kabul, Afghanistan
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc. --><path d="M215.7 499.2C267 435 384 279.4 384 192C384 86 298 0 192 0S0 86 0 192c0 87.4 117 243 168.3 307.2c12.3 15.3 35.1 15.3 47.4 0zM192 128a64 64 0 1 1 0 128 64 64 0 1 1 0-128z"/></svg>
</h4>
<div id="text">
  <h5>Wind Speed</h5>
<h3>10.3 km/h</h3>

<h5>Humidity</h5>
<h3>50%</h3>
</div>
<span  class='dem numb'><h3 style="display:inline;">22</h3 >  <span  class='s'> &#8451</span></span>
<input type="submit" id="submit" value="Search">

  </div>
</template>

<script>
// import {xmlhttpRequest} from '../../public/callapi.js';

// let obj=new xmlhttpRequest();
// obj.makeRequest()





  export default {
    
  }
</script>

<style scoped>
h4 svg{
  width: 1.3em;
    position: absolute;
    top: -0.2em;
    left: 1em;
    fill: #fff;

}
#submit{
    position: relative !important;
    top: 0px !important;
    cursor: pointer !important;
    border: 1px solid #03A9F4 !important;
    border-radius: 1em !important;
    height: 3em !important;
    transition: all .2s ease-in !important;
}
#submit:hover{
background: #e7e7e7;
color: #333;
border: none !important;
}
.dem{
  color: #fff;
    position: absolute;
    top: 9em;
    font-size: 3em;
}
.s{
font-size: .5em;
}
#dashbord{
  width: 26%;
  position:fixed;
    display: grid;
    box-shadow: -1px -3px 19px #4f4c4ba1;
    height: 49vw;
    -webkit-backdrop-filter: blur(10px);
    backdrop-filter: brightness(.5);
    justify-content: center;
    justify-items: center;
    align-content: space-evenly;

}
#dashbord input {
  height: 2em;
    background: #e7e7e73d;
    outline: none;
    width: 18em;
    border: none;
    border-radius: .5em .5em 0 0;
    border-bottom: 1px solid;
    color: #fff;
    padding: .4em 1em;
    position: relative;
    top: 4em;
    transition: all .2s ease-in;

}
div#text{
  font-family: sans-serif;
    width: 100%;
    color: #fff;
    position: relative;
    bottom: 5em;
    text-align: center;
}

::placeholder {
  color: #fff;
  opacity: 1; /* Firefox */
}

::-ms-input-placeholder { /* Edge 12 -18 */
  color: #fff;
}
h4{
  text-align: center;
  width: 100%;
    color: #fff;
    text-transform: capitalize;
    font-size: 0.9em;
    position: relative;
    font-family: sans-serif;
    border-bottom: 3px white solid;
    padding-bottom: .5em;
    height: 1.4em;
    bottom: 9em;

}#dashbord input[type='text']:focus{
  border-bottom: 2px solid #2196F3;
    background: #333;
}


@media only screen and (max-width:1200px) {
  #dashbord{
    height: 60vw;
  }
  h4{
    font-size: .7em;
    bottom: 11em;
  }
  input#search{
width: 15em !important;
  }
#text{
  bottom: 9em !important;
}
.dem{
  top: 7.5em !important;
}
#submit[type='submit']{
  top:-8em !important;
}

}
@media only screen and (max-width:1100px) {
  #dashbord{
    height: 58vw;
  }
  #submit[type='submit']{
  top:-4em !important;
}
  #text{
    bottom:7em !important
  }
  h4{
    font-size: .7em;
  }
  input#search{
width: 15em !important;
  }
}
@media only screen and (max-width:1000px) {
  #dashbord{
    height: 70vw;
  }
  #submit[type='submit']{
  top:-4em !important;
  width:100%;
}
  h4{
width:80%;
    font-size: .7em;
  }
  input#search{

width: 12em !important;
  }
  
}
@media only screen and (max-width:830px) {
  #dashbord{
    height: 79vw;
    width: 35%;
  }
  #submit[type='submit']{
  top:-4em !important;
  width:90%;
}
#text{
font-size: .6em;
bottom: 12em !important;
}
  h4{
width:80%;
    font-size: .6em;
  }
  input#search{

width: 10em !important;
  }

}
@media only screen and (max-width:740px) {
  #dashbord{
    height: 90vw;
    width: 35%;
  }
  #submit[type='submit']{
  top:-4em !important;
  width:90%;
}
#text{
font-size: .6em;
bottom: 12em !important;
}
  h4{
width:80%;
    font-size: .6em;
  }
  input#search{

width: 10em !important;
  }

}
@media only screen and (max-width:640px) {
  #dashbord{
    height: 110vw;
    width: 100%;
  }
 
#text{
font-size: .6em;
bottom: 17em !important;
}
  h4{
width:80%;
    font-size: .6em;
    bottom: 18em;
  }
  input#search{
top: 0;
width: 10em !important;
  }

}








</style>