
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

  <main>
    <div>

    </div>

    <div>
      <h4> Latest work</h4>

    </div>

    <div>
      <h4> Testimonial</h4>

    </div>

  </main>

  <footer>
    <div class="footerContent">
      <div class="footerText">
      <h3> Lets work together</h3>
      <p> This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com</p>

      <div class="footerImges">
        <img :src="imgDiscord"/>
        <img :src="imgFacebook"/>
        <img :src="imgDribble"/>
        <img :src="imgInstagram"/>
        <img :src="imgBehance"/>
      </div>

    </div>

    <form id="inputform" class="inputform">
      <input type="text" value="Name">
      <input type="email" value="Email">
      <input type="submit" class="inputSubmit" value="Submit">
    </form>
    </div>

  </footer>

</template>

<script>
  import imgLogo from "./assets/logoLogo.png"

  import imgHead from "./assets/logoHeader.png"
  import imgGoogle from "./assets/logo0google.png"
  import imgNike from "./assets/logo1nike.png"
  import imgSlmsung from "./assets/logo2slmsung.png"
  import imgAple from "./assets/logo3Apple.png"
  import imgAdidas from "./assets/logo4adidas.png"

  import imgDiscord from "./assets/socialdiscord.png"
  import imgFacebook from "./assets/socialfacebook.png"
  import imgDribble from "./assets/socialdribbble.png"
  import imgInstagram from "./assets/socialInstagram.png"
  import imgBehance from "./assets/socialbehance.png"
  
  export default {
    data(){
      return {
        products: ["Шоколад", "Пончик","Жвачка", "Мармелад", "Газировка"],
        imgLogo: imgLogo,

        imgHead: imgHead,
        imgGoogle: imgGoogle,
        imgNike: imgNike,
        imgSlmsung: imgSlmsung,
        imgAple: imgAple,
        imgAdidas: imgAdidas,

        imgDiscord: imgDiscord,
        imgFacebook: imgFacebook,
        imgDribble: imgDribble,
        imgInstagram: imgInstagram,
        imgBehance: imgBehance,

      }
    }
  }
</script>


<style scoped>
  body{
    display: flex;
    flex-wrap: wrap;
    width: 100%;

    p{
      font-size: 17px;
    }
    h6{
      font-size: 20px;
    }
    h1{
      font-size: 68px;
    }
    h3{
      font-size: 32px;
    }

    button{
      color: white;
      background-color: black;
      font-size: 20px;
      width: 211px;
      height: 78px;
    }
  }

  main{
    display: flex;
    flex-direction: column;

  }

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
    padding: 10px;
    img{
      height: 100%;
    }

  }

  .footerContent{
    display: flex;
    justify-content: space-between;
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;

  }

  .footerText{
    width: 570px;
    margin-right: 10%;

  }

  .footerImges{
    display: flex;
    
  }
  .inputform{
    display: flex;
    flex-direction: column;

    width: 520px;
    padding: 10px;
    input{
      font-size: 17px;
      background-color: #F3F3F3;
      color: #2D2D2D;
      border: none;
      padding: 10px;
      width: 100%;
      height: 59px;
    }
    .inputSubmit{
      color: white;
      background-color: black;
      font-size: 20px;
      width: 199x;
      height: 78px;
    }

  }

</style>