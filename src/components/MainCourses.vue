<script >
 
 export default {
    name:'MainCourses',
    data() {
        
        return
    }
 }
</script>

<template>
    <div class="container">
        <div class="wave-bot">
            <img src="../../edu/svg/svg-0.svg" alt="">

        </div>
        <div class="wave-top">
            <img src="../../edu/svg/svg-1.svg" alt="">
        </div>


        <div class="top-container">        
            <div class="left">
                
                <div>
                    <img src="../../edu/img/Books-icon.png" alt="">
                </div>

                <h1>
                    Thousand of courses for any type of student
                </h1>

                <p>
                    At EduPrime, it doesn't matter what domain you wish to pursue a career in.
                    here you can find a course that satisfies your needs within a click always
                    and applies foe a coursein a matter of minutes. EduPrime is ranked as the 
                    most versatile university in the world, thanks to the numer of courses it provides


                </p>

                <span class="button">
                    Browse through courses
                </span>
                
            </div>

            <div class="right">
                <div class="img">
                    <img src="../../edu/img/Graduation-Illustration.png" alt="">
                </div>
            </div>

        </div>
        <div class="bottom-container">
            <h1>Faculties available at EduPrime</h1>
            <span>A single university with a load of courses, tailored to satisfy any student's needs</span>
        </div>

      
    
    <div class="menu">

        <div class="img-container red">
            <img class="invert" src="../../edu/img/Gavel-v2.png" alt="">
        </div>

        <div class="img-container">
            <img src="../../edu/img/Coins-tabs-v2.png" alt="">
        </div>

        <div class="img-container">
            <img src="../../edu/img/Medicine-tabs-v2.png" alt="">

        </div>

        <div class="img-container">
            <img src="../../edu/img/Computer-tabs-v2.png" alt="">

        </div>

        <div class="img-container">
            <img src="../../edu/img/Palette-tabs-v2.png" alt="">

        </div>
        
       

    </div>

   </div> 
 
</template>

<style lang="scss" scoped>

@use '../styles/General.scss';
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;



.container{
    margin-top: 150px;
    margin-bottom: 150px;
    position: relative;
        .wave-bot{
            position: absolute;
            bottom: -155px;
            left: 0;
            
        }

    .wave-top{
        position: absolute;
        left: -27px;
        top: -160px;

    }

  
}
.top-container{
    @include flex ($type: 'both');
    color: #3d404f;
    

    .left{
        
        padding-right: 90px;
        padding-bottom: 50px;
        
        img{
            width: 70px;
        }

        h1{
            font-size: 50px;
            
            line-height: 60px;
            margin-bottom: 50px;

        }

        p{
            line-height: 30px;
            margin-bottom: 50px;
        }

        .button{
            margin: 0 ;
        }

        
    }

    .right{
        img{
            width: 570px;
        }
    }
}

.bottom-container{
    text-align: center;
    color: #3d404f;
    h1{
        margin-bottom: 30px;
        font-size: 50px
    }
    
    span{
        width: 380px;
        display: inline-block;
      
    }
}

.menu{
    width: 100rem;
    border: 1px solid lightgrey;
    box-shadow:2px 1px 5px grey ;
    height: 150px;
    margin-bottom: 50px;
    display: flex;
    padding: 0 10%;

    .img-container{
        width: calc(100% / 5);
        @include flex($type:'both');
        justify-content: space-around;
        border: 1px solid lightgray;
        
        img {
            width: 50%;
            
        }

        .invert{
            filter: grayscale(100%)
        }
    }        
    .red{
        background-color:  #d86b6e ;
        
    }
    }



</style>
