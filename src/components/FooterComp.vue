
<template>
    
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

  import imgDiscord from "../assets/socialdiscord.png"
  import imgFacebook from "../assets/socialfacebook.png"
  import imgDribble from "../assets/socialdribbble.png"
  import imgInstagram from "../assets/socialInstagram.png"
  import imgBehance from "../assets/socialbehance.png"
  
    
    export default {
      data(){
        return {  

          imgDiscord: imgDiscord,
          imgFacebook: imgFacebook,
          imgDribble: imgDribble,
          imgInstagram: imgInstagram,
          imgBehance: imgBehance,
  
        }
      },
      methods:{
        handeleubmit(){
            alert("Регистрация")
        },
    }
    }
  </script>
  
  
  <style scoped>
   
  
    .footerContent{
      display: flex;
      justify-content: space-between;
      /* position: fixed; */
      bottom: 0;
      left: 0;
      margin-bottom: 0;
      width: 100%;
      background-color: white;
  
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