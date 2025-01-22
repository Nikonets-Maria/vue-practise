
<template>

  <HeaderComp></HeaderComp>
  <MainComp></MainComp>
  <FooterComp></FooterComp>

</template>

<script>

import HeaderComp from "./components/HeaderComp.vue"
import FooterComp from "./components/FooterComp.vue"
import MainComp from "./components/MainComp.vue"
  
  export default {
    components:{
      HeaderComp,
      FooterComp,
      MainComp
    },

    data(){
      return {
      }
    },
  }
</script>


<style scoped>
  body{
    display: flex;
    height: 100vh;
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
    position:fixed;
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