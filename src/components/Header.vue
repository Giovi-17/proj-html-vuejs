<template>
    
  <div class="background">

    <img class="background-image" src="../assets/img/theme_slider2_bg-1.jpg" alt="background-image-graduation-hat">
    <img class="background-image-normal" src="../assets/img/Wave-1.png" alt="background-image-wave">

    <div class="container-fluid container-ms">

        <div class="row header-top d-flex align-items-center">

            <div class="col-3 logo d-flex justify-content-center align-items-center">

                <img src="../assets/img/theme_eduprime_logo.png" alt="logo">

            </div>

            <div class="col-9 nav-ms d-flex justify-content-end align-items-center">

                <div class="row container-info-courses align-items-center">

                    <div class="col-7 info">

                        <ul class="d-flex justify-content-end align-items-center">

                            <li v-for="(infoData, index) in headerD.headerDataInfo" :key="index" >{{ infoData }} <i class="fas fa-caret-down"></i></li>

                        </ul>

                    </div>

                    <div class="col-2 courses">

                        <ul class="d-flex justify-content-start align-items-center">

                            <li v-for="(infoData, index) in headerD.headerDataCourses" :key="index" >{{ infoData }}</li>

                        </ul>

                    </div>

                    <div class="col-3 btn-container justify-content-end">

                        <button type="button" class="btn btn-dark btn-lg btn-ms">VIEW COURSES</button>

                    </div>

                </div>

            </div>

        </div>

        <div class="row header-central d-flex space-layout-header d-flex justify-content-center">

            <div class="title d-flex justify-content-center">

                <h2>Key to yout success</h2>
                
            </div>

            <div class="content d-flex justify-content-center">

                <p>
                    EduPrime is the most versatile WordPress 
                    theme for education purposes,
                    showcasing universities,courses,
                    secondary schools etc.
                </p>

            </div>

            <div class="btn-container">

                <button type="button" class="btn btn-dark btn-lg btn-ms"><span><i class="fas fa-search"></i></span> Search courses</button>

                <button type="button" class="btn btn-dark btn-lg btn-ms btn-ms-two"><span><i class="fas fa-user-plus"></i></span> Apply for university</button>

            </div>

        </div>

    </div>

    <div class="side-menu">

        <div><i class="fas fa-shopping-cart"></i></div>

        <div><i class="far fa-newspaper"></i></div>

        <div><i class="far fa-check-circle"></i></div>

    </div>

  </div>

</template>

<script>
import "../assets/color.scss";

export default {
  name: "Header",
  props: {

    headerD: Object,

  }
};
</script>

<style lang="scss" scoped>

// General Color
$firstColor: white;
$secondColor: #e9d758;
$thirdColor: #da5f60e6;
$fourthColor: #8B8B8A;
$fifthColor: #e56768;
$sixthColor: #F7F8FA;
$seventhColor: #454545; 
//

.background{

    width: 100%;
    max-height: 700px;
    background-color: $fifthColor;
    position: relative;

    &-image{

        width: 100%;
        opacity: 10%;
        z-index: 1;
        max-height: 700px;
        object-fit: cover;

    }

    &-image-normal{

        width: 110%;
        position: absolute;
        bottom: 0;
        left: 0;
        z-index: 1;

    }

    .container-ms{

        width: 100%;

        z-index: 2;

        position: absolute;
        top: 0;
        left: 0;

        padding-top: 40px;

        .header-top{

            width: 100%;
            height: 100%;

            .logo{

                height: 100%;

                img{

                    width: 70%;
                    min-width: 190px;

                }

            }

            .nav-ms{

                height: 100%;

                .container-info-courses{

                    width: 100%;

                    .info{

                        height: 100%;

                    }

                    ul{

                        height: 100%;


                        li{

                            height: 100%;
                            display: flex;
                            align-items: center;
                            color: $firstColor;
                            margin: 0 15px;
                            font-size: 15px;

                            i{

                                font-size: 10px;
                                margin-left: 10px;

                            }

                        }

                        li:hover{

                            color: $secondColor;

                        }

                    }

                    .courses{

                        height: 100%;

                    }

                    .btn-container{

                        .btn-ms{

                            background-color: $secondColor;
                            border: $secondColor;
                            color: $firstColor;

                            margin-right: 30px;

                        }

                    }

                }

            }

        }

        .header-central{

            width: 100%;
            color: $firstColor;
            text-align: center;
            position: absolute;

            /*test*/
            top: 150%;
            left: 0;

            .title{

                width: 100%;
                margin: 15px 0;
                
                h2{

                    font-size: 45px;

                }

            }

            .content{

                width: 85%;
                max-width: 600px;
                margin: 15px auto;

            }

            .btn-container{

                .btn-ms{

                    background-color: $secondColor;
                    border: $secondColor;
                    color: $firstColor;

                    margin-right: 30px;

                }

                .btn-ms-two{

                    background-color: $firstColor;
                    border: $firstColor;
                    color: $fifthColor;

                }

                .btn-ms-two:hover{

                    background-color: $fifthColor;
                    border: $fifthColor;
                    color: $firstColor;

                }

                span{

                    i{

                        font-size: 13px;

                    }

                }

            }

        }

    }

    .side-menu{

        display: inline-block;
        background-color: $secondColor;
        padding: 5px;
        border-top-right-radius: 5px;
        border-bottom-right-radius: 5px;
        box-shadow: 0 0 20px 0px rgba(0, 0, 0, 0.4);

        position: absolute;
        top: 50%;
        left: 0;

        transform: translateY(-50%);

        z-index: 3;

        div{

            margin: 5px;

        }

        i{

            cursor: pointer;
            color: $firstColor;

        }

    }

}

</style>