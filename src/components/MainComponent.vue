<template>
    <div class="menu">
        <div class="menuList">
            <div class="menuItem">
                <ul>
                    <li>Головна</li>
                    <li>Каталог</li>
                    <li>Блог</li>
                    <li>Улюблене</li>
                    <li>Корзина</li>
                    <li>Контакти</li>
                </ul>
            </div>
        </div>
    </div>
    <div class="mainComponent">
      
        <swiper
            :spaceBetween="30"
            :effect="'fade'"
            :modules="modules"
            :autoplay="Autoplay"
            class="mySwiper"
        >
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake1.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake2.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake3.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake4.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake5.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake6.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake7.jpg"/>
            </swiper-slide>
   
        </swiper>
    </div>
    <div class="textBlock">
            <swiper
            :spaceBetween="30"
            :effect="'fade'"
            :modules="modules"
            :autoplay="Autoplay"
            class="mySwiper"
        >
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake1.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake2.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake3.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake4.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake5.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake6.jpg"/>
            </swiper-slide>
            <swiper-slide>
                <img src="@/assets/mainPageImg/cake7.jpg"/>
            </swiper-slide>
   
        </swiper>
        <div class="home">
            <div class="homeWrapper">
                <div class="info">
                    <div class="infoWrapper">
                        <div class="title">
                            <h1>Cолодка майстерня авторських солодощів</h1>
                        </div>
                        <div class="subTitle">
                            <h4> by Natali</h4>
                        </div>
                        </div>
                </div>
                <div class="order">
                    <div class="orderWrapper">
                        <h2>Замовити</h2>
                        <div class="input">
                            <input type="text" class="input1" placeholder="Ваше ім'я"/>
                            <i class="fa-solid fa-envelope"></i>
                        </div>
                        <div class="input">
                            <input type="text" class="input1" placeholder="Ваш контактний телефон"/>
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        <div class="input">
                            <input type="text" class="input1" placeholder="Деталі замовлення"/>
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        <div class="button">
                            <button>Замовити</button>
                        </div>
                    </div>

                </div>
            </div>

        </div>
       

        </div>
    <div class="buttonBar">
        <div class="likeBtn">
            
        </div>

        <div class="instBtn">

        </div>
        <div class="store">

        </div>
        <div class="plusBtn">
            
        </div>

    </div>
</template>

<script>

import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/effect-fade';
import 'swiper/css/navigation';
import 'swiper/css/pagination';

// import '../../assets/scss/main.scss';

// import required modules
import { EffectFade, Autoplay
    //  Navigation, Pagination 
    } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectFade, Autoplay
    //    Navigation, Pagination
    ],
        Autoplay: {
            delay: 5000,
        },
    };
  },
};





// export default {

// }
</script>

<style lang="scss">
@import '@/assets/style/main.scss';
// 
.menu {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(3px);
    position: absolute;
    z-index: 3;
    width: -webkit-fill-available;
    height: 10vh;
    .menuItem{
        display: flex;
        justify-content: center;
        ul{
            margin: 0 5px;
            padding: 0;
            width: -webkit-fill-available ;
            text-align: center;
            // li::before{
            //     border: 1px solid white;
            // }
            li{
                padding: 1vh 0;
                margin: 0.5vh 1vw;
                border: 1px solid transparent;
                transition: all ease 0.5s;
                display: inline-block;
                width: 10vw;
                list-style-type: none;
                // display: inline-block;
                font-size: 2vh;
                color: white;
            }
            li:hover{
                cursor: pointer;
                border: 1px solid white;
                transition: all ease 0.5s;
                // border-top-width: 20%;
                // border-bottom-width: 20%;
                background-color: rgba(0, 0, 0, 0.4);
            }
        }

    }
    
}
.mainComponent{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 105vh;
    z-index: 1;
    position: relative;
    --mask:
    radial-gradient(50.39px at 50% calc(100% - 68.75px),#000 99%,#0000 101%) calc(50% - 50px) 0/100px 100%,
    radial-gradient(50.39px at 50% calc(100% + 43.75px),#0000 99%,#000 101%) 50% calc(100% - 25px)/100px 100% repeat-x;
    -webkit-mask: var(--mask);
          mask: var(--mask);
  
    .swiper{
        .swiper-slide{

            img{
                filter: blur(8px) brightness(0.9);
                width: 100vw;
                height: 105vh;
                max-height: 105vh;
            }
        }
    }
}
.textBlock{
        // position: absolute;
        // color: white;
        // z-index: 2;
        // // width: -webkit-fill-available;
        // // height: 100vh;
        //     width: 80vw;
        // height: 60vh;
        // display: flex;
        // justify-content: center;
        // align-items: center;
        position: absolute;
        top: 55%;
        left: 50%;
        width: 80vw;
        height: 80vh;   
        transform: translate(-50%, -50%);
        background-position: center;
        background-size: cover;
        display: flex;
        border: 1px solid black;
        border-radius: 10px;
        border: none;
        z-index: 1;
        // border: 1px solid white;
        // border-radius: 2vw;
        .title{
            max-width: 50vw;
            text-align: center;
        }
        .swiper{
        .swiper-slide{
            img{
                filter: brightness(0.7);
                object-fit: cover;
                // width: 100vw;
                height: -webkit-fill-available;
                // border: 1px solid white;
                // border-radius: 2vw;
            }
        }
        
    }
    .home{
        width: -webkit-fill-available;
        height: -webkit-fill-available;
            position: absolute;
            z-index: 1;
        }
        .homeWrapper{
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: baseline;
            .info{
                // display: inline-block;
                position: relative;    
                width: 70%;
                height: inherit;
                .infoWrapper{
                    display: flex;
                    flex-direction: column;
                    justify-content: space-between;
                    width: 100%;
                    height: 100%;
                    .title{
                        display: inherit;
                        justify-content: center;
                        h1{
                            padding: 2vh;
                            background-color: rgba(0,0,0, 0.4);

                            border: 1px solid white;
                            margin: 1.5vh 0;
                        }
                    }
                    .subTitle{
                        display: inherit;
                        justify-content: flex-end;
                        h4{
                            padding: 2vh;
                            background-color: rgba(0,0,0, 0.4);

                            border: 1px solid white;
                            margin: 1.5vh 4vw;
                        }


                    }
                }
            }
            .order{
                // display: inline-block;
                position: relative;
                backdrop-filter: blur(20px);
                width: 30%;
                height: -webkit-fill-available;
                padding: 2vh 2vw;
                // border: 1px solid;
                // border-radius: 0 2vw 2vw 0;
                .orderWrapper{
                    display: flex;
                    justify-content: center;
                    flex-direction: column;
                    align-items: center;
                    height: inherit;
                    h2{
                        text-align: center;
                        margin-bottom: 20px;
                        color: white;
                        position: relative;
                        bottom: 5vh;
                    }
                    .input{
                        position: relative;
                        width: 100%;
                        height: 30px;
                        margin-bottom: 7vh;
                        .input1{
                            // font-size: 16px;
                            display: flex;
                            flex-direction: column;
                            justify-content: center;
                            align-items: center;
                            background: transparent;
                            border: none;
                            outline: none;
                            border-bottom: 2px solid #fff;
                            color: white;
                            width: 100%;
                            height: 100%;
                        }
                        
                    }
                    .button{
                        width: 80%;
                        height: 5vh;
                        button{
                            width: 100%;
                            background-color: rgb(247, 16, 16);
                            height: 5vh;
                            border: none;
                            color: white;
                            font-size: 16px;
                            border-radius: 5px;
                        }

                    }
                }

            }
        }
        
    }


</style>
