
<template>

    <header>
      <div class="headerLine">
        <img :src="imgLogo"/>
        <div class="headerLinks">
          <p>About</p>
          <p>Work</p>
          <p>Contact</p>
        </div>
        
      </div>
  
      <div class="headerContent">
        <div class="headerText">
          <h6> Branding | Image making</h6>
          <h1> Visual Designer </h1>
          <p> This is a template Figma file, turned into code using Anima. 
            Learn more at AnimaApp.com </p>
          <button>Contact</button>
        </div>
        
        <img :src="imgHead"/>
      </div>
      
      <div class="logosWraper">
        <img :src="imgGoogle"/>
        <img :src="imgNike"/>
        <img :src="imgSlmsung"/>
        <img :src="imgAple"/>
        <img :src="imgAdidas"/>
  
      </div>
    </header>
  
  </template>
  
  <script>
    import imgLogo from "../assets/logoLogo.png"
  
    import imgHead from "../assets/logoHeader.png"
    import imgGoogle from "../assets/logo0google.png"
    import imgNike from "../assets/logo1nike.png"
    import imgSlmsung from "../assets/logo2slmsung.png"
    import imgAple from "../assets/logo3Apple.png"
    import imgAdidas from "../assets/logo4adidas.png"

    export default {
      data(){
        return {
          imgLogo: imgLogo,
          imgHead: imgHead,
          imgGoogle: imgGoogle,
          imgNike: imgNike,
          imgSlmsung: imgSlmsung,
          imgAple: imgAple,
          imgAdidas: imgAdidas,
        }
      }
    }
  </script>
  
  
  <style scoped>
 
  
    .headerLine{
      display: flex;
      justify-content: space-between;
    }
  
    .headerLinks{
      
      display: flex;
      justify-content: end;
    }
  
    .headerContent{
      display: flex;
      margin-top: 20px;
      justify-content: space-between;
  
    }
  
    .headerText{
      width: 40%;
  
    }
  
    .logosWraper{
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px;
      img{
        height: 100%;
      }
  
    }
    
  
  </style>