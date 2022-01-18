<template>
    
  <div class="background">

    <div class="backgroundImage">

      <img src="../assets/img/home-background.png" alt="decoration">

    </div>

    <div class="space-layout-general">

      <div class="row">

        <div class="col-6 sectionCol">

          <div class="mini-img-section">

            <img src="../assets/img/Books-icon.png" alt="books">

          </div>

          <div class="title d-flex">
            
            <h2>Thousands of courses for any type of student</h2>
            
          </div>

          <div>

            <p class="content d-flex justify-content-center">
              
              At EduPrime, it doesn't matter what domain you wish
              to pursue a career in. Here you can find a course that 
              satisfies your needs within a click away and applies for 
              a course in a matter of minutes. EduPrime is ranked as 
              the most versatile univeristy in the world, thanks to 
              the number of courses it provides.
            
            </p>
            
          </div>

          <div class="btn-container">

            <button type="button" class="btn btn-dark btn-lg btn-ms"><span>Browse through courses</span></button>

          </div>

        </div>

        <div class="col-5 offset-1 sectionCol">

          <img src="../assets/img/Graduation-Illustration.png" alt="decoration">

        </div>

      </div>

    </div>

    <div class="space-layout-general">

      <div class="title d-flex justify-content-center">
            
        <h2>Faculties available at EduPrime</h2>
            
      </div>

      <div>

        <p class="content content-space d-flex justify-content-center">
              
          A single university with a load of courses, tailored to satisfy any student's needs.
            
        </p>
            
      </div>

    </div>

    <div class="facultiesContainer">



    </div>

    <div class="space-layout-section-main">

      <div class="row d-flex justify-content-evenly">

        <div class="col-6 sectionCol">

          <img src="../assets/img/Gavel-Illustration-e1556884768193.png" alt="decoration">

        </div>

        <div class="col-5 offset-1 sectionCol">

          <div class="title d-flex">
            
            <h3>Law Faculty</h3>
            
          </div>

          <div>

            <p class="content d-flex justify-content-center">
              
              Learning from world-leading academics and practitioners,
              you'll not only receive an outstanding grounding in the
              theory of law, but you will be able to understand
              how those principles are applied in practice through
              a range of student-led activities and competitions.
            
            </p>
            
          </div>

          <div class="btn-container">

            <button type="button" class="btn btn-dark btn-lg btn-ms"><span>Read More</span></button>

          </div>

        </div>

      </div>

    </div>

    <div class="wave">

      <img src="../assets/svg/svg-0.svg" alt="decoration">

    </div>

    <div class="background-space-layout-general">

      <div class="space-layout-general-marginZero">

        <div class="mini-img">

          <img src="../assets/img/Clock-and-Bell.png" alt="">

        </div>

        <div class="d-flex justify-content-center">

          <div class="title">

            <h3>University Year</h3>

          </div>

        </div>

        <div class="spaceMargin">
          
          <div class="row">

            <div class="col-3 offset-3">

              <div class="colTitle">

                <span>Demo Classes</span>

              </div>

              <div class="colP">
                
                <span>
                  
                  In the first week, students try to accommodate
                  with the teaching style and choose their 
                  optional courses.
                  
                </span>
                
              </div>

            </div>

            <div class="col-3 offset-2">

              <div class="colTitle">

                <span>Graduation Day</span>

              </div>

              <div class="colP">
                
                <span>
                  
                  On the day of graduation, all students gather 
                  for the ceremony and then network and 
                  party among others. 
                  
                </span>
                
              </div>

            </div>

          </div>

        </div>

        <div class="graphic">

          <img src="../assets/img/Timeline-Item.png" alt="">

        </div>

        <div class="spaceMargin">
          
          <div class="row">

            <div class="col-3 offset-1">

              <div class="colTitle">

                <span>Orientation</span>

              </div>

              <div class="colP">
                
                <span>
                  
                  First day of the university year, all students 
                  gather for the opening ceremony and then 
                  network with others.
                  
                </span>
                
              </div>

            </div>

            <div class="col-3 offset-2">

              <div class="colTitle">

                <span>Evaluation</span>

              </div>

              <div class="colP">
                
                <span>
                  
                  At the end of a semester, students take a 
                  general evaluation test for every subject 
                  they're learning.
                  
                </span>
                
              </div>

            </div>

          </div>

        </div>

        <div class="background-space-layout-general">

          <div class="space-layout-general-marginZero">

            <div class="space-layout-general-marginZero">

              <div class="mini-img">

                <img src="../assets/img/upcoming-events-calendar-icon.png" alt="">

              </div>

            <div class="d-flex justify-content-center">

              <div class="title-two">

                <h3>Upcoming Events</h3>

              </div>

            </div>

          </div>

        </div>

      </div>

    </div>

  </div>

  </div>

</template>

<script>
import "../assets/color.scss";

export default {
  name: "Main",
};
</script>

<style lang="scss" scoped>

// General Color
$firstColor: white;
$secondColor: #e9d758;
$thirdColor: #da5f60e6;
$fourthColor: #8B8B8A;
$fifthColor: #e56768;
//

  .background{

    background-color: $firstColor;
    margin-top: 50px;

    img{

      width: 100%;

    }

    .backgroundImage{

      width: 100%;

      z-index: 1;

      img{

        /*Test*/
        width: 100%;

        display: none;

      }

    }

    .background-space-layout-general{

      background-color: $fifthColor;

    }

    .space-layout-general, .space-layout-section-main, .space-layout-general-marginZero{

      z-index: 2;
      margin: 100px 0;

      .content{

        margin: 20px 0;
        font-size: 13px;

      }

      .content-space{

        padding: 0 35%;
        text-align: center;

      }

      .sectionCol{

        img{

          width: 100%;

        }

        .mini-img-section{

          width: 50px;
          margin-bottom: 10px;

          img{

            width: 100%;

          }

        }

        .btn-container{

          justify-content: start;

          .btn-ms{

            background-color: $secondColor;
            border: $secondColor;
            font-size: 12px;

          }

        }

      }

    }

    .wave{

      width: 100%;

      img{

        width: 150%;
        position: relative;
        top: 3px;

      }
        
    }

    .space-layout-section-main{

      padding: 0 20%;

      .content{

        color: $fourthColor;

      }

      .sectionCol{

        .btn-container{

          .btn-ms{

            background-color: $thirdColor;
            border: $thirdColor;
            font-size: 13px;

          }

        }

      }

    }

    .space-layout-general-marginZero{

      margin: 0;
      padding: 60px 15%;
      color: $firstColor;
      position: relative;

      .spaceMargin{

        margin: 50px 0;

      }

      .mini-img{

        width: 50px;

        position: absolute;
        top: 0;
        left: 50%;

        transform: translateX(-50%);

      }

      .title{

        text-align: center;
        margin-bottom: 50px 0;

        width: 250px;
        
        h3{

          font-size: 35px;

          background-color: red;

        }

      }

      .title-two{

        margin-bottom: 50px 0;


        h3{

          font-size: 35px;

          background-color: transparent;

        }

      }

      .graphic{

        margin: 50px 0;

      }

      .colTitle{

        font-weight: bold;

        text-align: center;

      }

      .colP{

        text-align: center;

        font-size: 13px;

      }

    }

  }

</style>