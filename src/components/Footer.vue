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

      <div class="col-4 search">

        <div class="searchBar">

          <div class="btn-container">

            <div class="searchBarSpan d-flex btn-ms">

              <span>Search ...</span>

              <div class="searchBarButton btn-container">
                
                <div class="btn-msR">

                  <i class="fas fa-search"></i>

                </div>
                
              </div>

            </div>

            

          </div>

        </div>

        <span class="searchCategories">Search categories</span>

        <div class="categories d-flex">

          <div v-for="(categories, index) in footerD.footerDataCategories" :key="index" class="btn-container">

            <div class="btn btn-ms">{{ categories }}</div>

          </div>

        </div>

        <span class="rights">ModelTheme, All rights reserved.</span>

      </div>

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
$fourthColor: #8B8B8A;
//

.background{

  background-color: $thirdColor;
  color: $firstColor;
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

    .search{

      text-align: right;

      .searchBar{

        display: block;

        margin-bottom: 15px;

        .btn-container{

          width: 100%;

          flex-direction: column;

          text-align: left;

          align-items: end;

          .searchBarSpan{

            position: relative;
            width: 100%;

          }

          .searchBarButton{

            position: absolute;
            top: 0;
            left: 0;

            .btn-msR{

              width: 62px;
              height: 62px;

              border-radius: 50%;

              text-align: center;

              background-color: $secondColor;
              border: $secondColor;
              color: $firstColor;

              font-size: 15px;

              padding: 20px 20px;

            }

          }

          .btn-ms{

            background-color: $firstColor;
            border: $firstColor;
            color: $fourthColor;

            font-size: 15px;

            padding: 20px 20px;

          }

        }

      }

      .searchCategories{

        font-weight: bold;

        margin: 15px 0;

      }

      .categories{

        flex-wrap: wrap;

        justify-content: end;

        margin: 15px 0;

        .btn-container{
          
          display: block;

          .btn-ms{

            border: 1px solid $firstColor;
            color: $firstColor;

            padding: 5px 15px ;
            font-size: 12px;

            margin: 5px 5px;
            text-transform: uppercase;

          }

        }

      }



      .rights{

        color: $secondColor;

      }

    }

  }

}

</style>