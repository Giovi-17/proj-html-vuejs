<template>
    
  <div class="background">

    <div class="row space-layout-general">

      <div class="col-4 social">

        <img src="../assets/img/theme_eduprime_logo.png" alt="logo">

        <p>EduPrime is the most versatile WordPress theme for educational purposes, showcasing universities, courses, secondary schools etc.</p>

        <ul class="d-flex">

          <li><i class="fab fa-facebook-f"></i></li>

          <li><i class="fab fa-twitter"></i></li>

          <li><i class="fab fa-instagram"></i></li>

        </ul>

      </div>

      <div class="col-4 link d-flex">

        <div class="link-container">

          <ul>

            <li class="title">Get EduPrime</li>

            <li v-for="(linkOneD, index) in footerD.footerDataLinkOne" :key="index" >{{ linkOneD }}</li>


          </ul>

        </div>

        <div class="link-container">

          <ul>

            <li class="title">Networking</li>

            <li v-for="(linkTwoD, index) in footerD.footerDataLinkTwo" :key="index" >{{ linkTwoD }}</li>

          </ul>
          
        </div>


      </div>

      <div class="col-4 search"></div>

    </div>

  </div>

</template>

<script>
import "../assets/color.scss";

export default {
  name: "Footer",
  props: {

    footerD: Object,

  }
};
</script>

<style lang="scss" scoped>

// General Color
$firstColor: white;
$secondColor: #e9d758;
$thirdColor: #da5f60e6;
//

.background{

  background-color: $thirdColor;
  color: $firstColor;
  /*test*/
  /* height: 500px; */
  padding: 120px 0;

  .space-layout-general{

    .social{

      img{

        width: 80%;

      }

      p{

        margin: 30px 0;

      }

      ul{

        li{

          display: flex;
          justify-content: center;
          align-items: center;
          width: 50px;
          height: 50px;
          margin: 0 5px;
          border: 3px solid $secondColor;
          padding: 10px;
          font-size: 20px;
          border-radius: 50%;
          cursor: pointer;

        }

      }

    }

    .link{

      .link-container{

        width: 50%;

        ul{

          .title{

            font-weight: bold;
            font-size: 20px;
            margin-bottom: 30px;


          }

          li{

            font-size: 15px;
            margin: 10px 0;

          }

        }

      }

    }

  }

}

</style>