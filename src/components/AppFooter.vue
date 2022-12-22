<script >
 export default {

    name:'AppFooter',
    data() {
       return {
         edu:
                [
                    {
                        title: "Get EduPrime",
                        list: [
                            {
                                name: "Request a web site",
                                href: "#"
                            },
                            {
                                name: "Browse themes",
                                href: "#"
                            },
                            {
                                name: "Payment options",
                                href: "#"
                            },
                            {
                                name: "Support Syste",
                                href: "#"
                            },
                            {
                                name: "Checkout",
                                href: "#"
                            },
                            {
                                name: "Purchase Theme",
                                href: "#"
                            },
                            
                        ],
                    },
                ],
            net: [
                {
                    title: "Net working",
                    list: [
                        {
                            name: "Purchase Theme",
                            href: "#"
                        },
                        {
                            name: "Our Benefits",
                            href: "#"
                        },
                        {
                            name: "Our Team",
                            href: "#"
                        },
                        {
                            name: "Our Service",
                            href: "#"
                        },
                        {
                            name: "Our product",
                            href: "#"
                        },
                        {
                            name: "My account",
                            href: "#"
                        },
                        
                    ]
                }
               ],

               search: [
                {
                    title: "Search categories",
                    list: [
                        {
                            name: "ECONOMY",
                            href: "#"
                        },
                        {
                            name: "DESIGN",
                            href: "#"
                        },
                        {
                            name: "COACHING",
                            href: "#"
                        },
                        {
                            name: "BUSINESS",
                            href: "#"
                        },
                        {
                            name: "MEDICINE",
                            href: "#"
                        },
                        {
                            name: "LAW",
                            href: "#"
                        },
                        {
                            name: "FITNESS",
                            href: "#"
                        }
                        
                    ]
                }
               ],
      }
   }
}

</script>

<template>
   <div class="container">
      <section class="side-menu">

      </section>

      <section class="social">
         <div class="img">         
            <img src="../../edu/img/theme_eduprime_logo.png" class="logo">
         </div>
         <span>
         EduPrime is the most versatile WordPress theme for educational purposes, 
         showcasing universities, courses, secondary school etc
         </span>
         <div class="social-link">

         </div>


      </section  >

      <section class="list-menu">
            <ul class="list">
               <li class="sub" v-for="(item, index) in edu" :key="index">
                     
                  <a href="" class="title-text "><h3>{{ item.title }}</h3></a>
                  <a :href="item.href" v-for="(items, index) in item.list">{{ items.name }} </a>

               </li>
            </ul>

            <ul class="list">
               <li class="sub" v-for="(item, index) in net" :key="index">
                     
                  <a href="" class="title-text "><h3>{{ item.title }}</h3></a>
                  <a :href="item.href" v-for="(items, index) in item.list">{{ items.name }} </a>

               </li>
            </ul>
         
      </section>
      
      <section class="search">
         <div class="input-src">
            <span class="input">Search...</span>
            <span class="icon-search"></span>
         </div>

         <ul class="list">
               <li class="sub" v-for="(item, index) in search" :key="index">
                     
                  <a href="" class="title-text "><h3>{{ item.title }}</h3></a>
                  <span class="Search-item"><a :href="item.href" v-for="(items, index) in item.list">{{ items.name }} </a></span>

               </li>
         </ul>

      </section>
      <section></section>
   </div>
 
</template>

<style lang="scss" scoped>

@use '../styles/General.scss' as *;
@use '../styles/partials/variables.scss' as *;

.container{

   display: flex;
   justify-content: space-between;
   align-items: center;
   background-color:#d86b6e ;
   min-height: 200px;
   padding: 2% 3%;

   section{
      height: 300px;
   }
   .social{
      width: calc(100% / 5);
      
   }
   img{
      margin-bottom: 10px;
   }

   span{
      line-height: 20px;
      color: $color-white;
   }

   .list-menu{
   display: flex;
   justify-content: space-between;
   align-items: center;

      .sub{
         display: flex;
         flex-direction: column;
         justify-content: start;
         margin: 0 40px;
         line-height: 40px;

         h3{
            margin-bottom: 20px;
         }

      }

   }

   .input-src{
      position: relative;
      display: flex;
      justify-content: start;
      align-items: center;
      background-color: $color-white;
      width: 350px;
      height: 80px;
      border-radius: 40px ;
      


      .input{
         color: #8b8b8a ;
         padding-left: 20px;
         font-size: 20px;
      }

      .icon-search{
         position: absolute;
         right: 0;
         background-color: #e9d758;
         width: 80px;
         height: 80px;
         border-radius: 50%;
      }

   }

   .search{
      display: flex ;
      flex-direction: column;
      align-items: flex-end;
      width: 450px;
      
      .sub{
         display: flex;
         flex-wrap: wrap;
         flex-direction: column;
         align-items: flex-end;
         line-height: 50px;

         .Search-item{
            display: flex;
            justify-content: end;
            flex-wrap: wrap;
            a{
               border: 1px solid white;
               margin: 5px;
               padding: 7px 12px;
               border-radius: 25px;

            }

         }
      }

      
     
     

     
   }


}

</style>
