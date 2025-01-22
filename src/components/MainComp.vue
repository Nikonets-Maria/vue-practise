
<template>

  
    <main class="content">
        <div class="serviceSechion">
            <div v-for="item in service" :key="item.id" class="serviceContent">
            <img :src="item.imgSrc"/>
            <h3> {{ item.title }}</h3>
            <p>{{ item.text }}</p>
            </div>
      </div>

      <h3> Latest work</h3>

      <div>
        <div class="gallerySechion">
            <div v-for="item in gallery" :key="item.id" class="galleryContent">
            
            <img :src="item.imgSrc"/>
            <h4> {{ item.title }}</h4>
            <p>{{ item.text }}</p>

        </div>
      </div>
  
      </div>

      <h3> Testimonial</h3>

      <div>
        <div class="cardsSechion">
            <div v-for="item in cards" :key="item.id" class="cardsContent">
                <p>{{ item.text }}</p>

                <div>
                    <img :src="item.imgSrc"/>
                    <img v-for="item in item.stars" :key="item.id" :src="imgStar"/> 
                   
                    <div>
                            <h5> {{ item.name }}</h5>
                            <p> {{ item.company }}</p>
                    </div>                  
                </div>
                    
                    
                </div>
            </div>
            
        
        </div>
        
    </main>
  
  
  </template>
  
  <script>
    import imgProduct1 from "../assets/ProductImage1.png"
    import imgProduct2 from "../assets/ProductImage2.png"
    import imgProduct3 from "../assets/ProductImage3.png"
    import imgProduct4 from "../assets/ProductImage4.png"
    import imgProduct5 from "../assets/ProductImage5.png"
    import imgProduct6 from "../assets/ProductImage6.png"

    import imgSkillCardPink from "../assets/SkillsCardIconPink.png"
    import imgSkillCardOrange from "../assets/SkillsCardIconOrange.png"
    import imgSkillCardGreen from "../assets/SkillsCardIconGreen.png"

    import imgClient from "../assets/ClientImg.png"
    import imgStar from "../assets/Star.png"

    export default {
      components:{
      },
  
      data(){
        return {
            // imgProduct1: ,
            // imgProduct2: ,
            // imgProduct3: ,
            // imgProduct4: ,
            // imgProduct5: ,
            // imgProduct6: ,

            // imgSkillCardPink: imgSkillCardPink,
            // imgSkillCardOrange: imgSkillCardOrange,
            // imgSkillCardGreen: imgSkillCardGreen,
            imgStar: imgStar,

            service: [ 
            {id: 1, imgSrc: imgSkillCardPink, title: 'Product Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 2, imgSrc: imgSkillCardOrange, title: 'Visual Design', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 3, imgSrc: imgSkillCardGreen, title: 'Art Direction', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}
            ],

            gallery: [
            {id: 1, imgSrc: imgProduct1, title: 'Project title', text: 'UI, Art drection'}, 
            {id: 2, imgSrc: imgProduct2, title: 'Project title', text: 'UI, Art drection'}, 
            {id: 3, imgSrc: imgProduct3, title: 'Project title', text: 'UI, Art drection'},  
            {id: 4, imgSrc: imgProduct4, title: 'Project title', text: 'UI, Art drection'}, 
            {id: 5, imgSrc: imgProduct5, title: 'Project title', text: 'UI, Art drection'},  
            {id: 6, imgSrc: imgProduct6, title: 'Project title', text: 'UI, Art drection'}, 
            ],

            cards: [
            {id: 1, imgSrc: imgClient, stars: 5, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 2, imgSrc: imgClient, stars: 5, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 3, imgSrc: imgClient, stars: 1, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 4, imgSrc: imgClient, stars: 2, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 5, imgSrc: imgClient, stars: 3, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 
            {id: 6, imgSrc: imgClient, stars: 4, name: 'Gemma Nolen', company: 'Google', text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com'}, 

        ],

        }
      },
    }
  </script>
  
  
  <style scoped>
  
  .content{
    display: flex;
    align-items: center;
}

  .serviceSechion{
    display: flex;
    justify-content: space-around;
  }
  .serviceContent{
    width: 395px;
    margin: 30px;
    padding: 64px, 42px;
    gap: 42px;
    text-align: center;
  }


    .gallerySechion{
        display: flex;
        align-items: center;
        justify-content: space-around;
        flex-wrap: wrap;
        
    }
    .galleryContent{
        width: 395px;
        gap: 24px;
        align-items: center;
        justify-content: space-between;
        img{
            width: 100%;
        }
    }
    .cardsSechion{
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
        /* margin-bottom: 300px; */
    }
    .cardsContent{
        display: flex;
        flex-direction: column;
        width: 30%;
        height: 330px;
        margin: 10px;
        padding: 42px;
        gap: 68px;
        background-color: #F3F3F3;
    }
   
  </style>