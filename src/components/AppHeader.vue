<script >

export default {
  name:'AppHeader',
   
   data() {
    
    return {
      link: [
          {
          name: "Home",
          href: "#"
          
          },

          {
          name: "Courses",
          href: "#"

          },

          {
          name: "About Us",
          href: "#"

          },

          {
          name: "News",
          href: "#"

          },

          {
          name: "Pages",
          href: "#"

          },

          {
          name: "Contact",
          href: "#"

          },

          {
          name: "Purchase",
          href: "#"

          },

      ]
    }
  }
}

</script>

<template>
  <header>
        <div class="container">
          <div class="side-menu"></div>
          <div class="header-top">

            <div class="left">
                <img src="../../edu/img/theme_eduprime_logo.png" alt="logo" class="logo">
            </div>

            <div class="right">
                
              <ul class="list">
                <li v-for="(item, index) in link" :key="index" >
                    <a href="">{{item.name}}</a>
                </li>
              </ul> 
            
              <span class="button yellow">
                VIEW COURSES 
              </span>

            </div>
          

          </div>
        

          <div class="header-bot">
            <h1>Key to your success</h1>
            <span>
              EduPrime is the most versatile WordPress theme for educational purposes, 
              showcasing universities, courses, secondary school etc
            </span>
            <div class="btns">
              <div class="button yellow">Search courses</div>
              <div class="button white">Apply for university</div>

            </div>
           

          </div>

        </div>

  </header>
 
</template>

<style lang="scss" scoped>
@use '../styles/General.scss' as *;
@use '../styles/partials/variables.scss' as *;

.container{
 
  background-color: #d86b6e;
  min-height: 400px;
  padding: 3% 5%;
  position: relative;
      .side-menu{
      position: absolute;
      left: 0;
      top: 250px;
      background-color: #e9d758;
      height: 80px;
      width: 25px;
      border-radius: 3px;
      box-shadow:2px 1px 5px grey ;
    }

    .header-top{
      display: flex;
      justify-content: space-between;
      align-items: center;
      
      

    }

    .right{
      display: flex;
      justify-content: space-between;
      align-items: center


    }

   
      .list{
      display: flex;
      justify-content: space-between;
      align-items: center;
      list-style-type: none;
      gap: 10px;

      a{
              text-decoration: none;
              color: $color-white;
              font-weight: bold;
              font-size: 20px;
              

      }
      
   

      }
   .button{
        background-color:#e9d758 ;
        padding: 15px 25px;
        margin: 15px;
        border-radius: 25px;
        font-weight: bold;
        color: $color-white;
        cursor: pointer;

        &:hover{
          background-color: $color-white ;
          color:#d86b6e
        }

        
        
        
        
      
        
      }
}


.header-bot{
  margin: 5% 30%;
  color: $color-white;

  h1{
    text-align: center;
    margin-bottom: 5%;
    font-size: 50px;
  }

  span{
    display: block;
    text-align: center;
    font-size: 20px;
    margin-bottom: 5%;

  }

  .btns{
    display: flex;
    justify-content: space-evenly;
    align-items: center;

    .white{
      background-color: $color-white;
      color: #e56768;
    }
  }

}





</style>

