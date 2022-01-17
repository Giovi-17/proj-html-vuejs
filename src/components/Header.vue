<template>
    
  <div class="background">

    <img class="background-image" src="../assets/img/theme_slider2_bg-1.jpg" alt="background-image-graduation-hat">
    <img class="background-image-normal" src="../assets/img/Wave-1.png" alt="background-image-wave">

    <div class="container-fluid container-ms">

        <div class="row header-top d-flex">

            <div class="col-3 logo d-flex justify-content-center align-items-center">

                <img src="../assets/img/theme_eduprime_logo.png" alt="logo">

            </div>

            <div class="col-8 offset-1 nav-ms d-flex justify-content-end">

                <div class="row container-info-courses">

                    <div class="col-5 info">

                        <ul class="d-flex justify-content-end align-items-center">

                            <li v-for="(infoData, index) in headerD.headerDataInfo" :key="index" >{{ infoData }}  <img class="arrow" src="../assets/img/back-to-top-arrow.svg" alt="arrow"></li>

                        </ul>

                    </div>

                    <div class="col-4 courses">

                        <ul class="d-flex justify-content-start align-items-center">

                            <li v-for="(infoData, index) in headerD.headerDataCourses" :key="index" >{{ infoData }}  <img class="arrow" src="../assets/img/back-to-top-arrow.svg" alt="arrow"></li>

                        </ul>

                    </div>

                    <div class="col-3 btn-container justify-content-end">

                        <button type="button" class="btn btn-dark btn-lg btn-ms">VIEW COURSES</button>

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
//

.background{

    width: 100%;
    background-color: #da5f60e6;
    position: relative;

    &-image{

        width: 100%;
        opacity: 10%;
        z-index: 1;

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
        height: 120px;

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
                                
                                .arrow{

                                margin-left: 5px;
                                width: 7px;
                                transform: rotate(180deg);

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

    }

}

</style>