<template>
    <div class="topDesertsBg">
        <div class="topDeserts">
            <div class="container">
                <div class="vector3">
                    <img src="@/assets/vector3.png" alt="vector3">
                </div>
                <div class="componentTitle">
                    <h1>Варто спробувати наші десерти</h1>
                </div>
                <div class="vector vectorDark">
                    <img src="@/assets/vector1.png" alt="vector">
                </div>
                <swiper
                    :slidesPerView="3"
                    :spaceBetween="30"
                    :navigation="{
                        prevEl: prevBtn,
                        nextEl: nextBtn,
                        }"
                    :modules="modules"
                    class="mySwiper"
                >
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/desert1.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/desert2.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/desert3.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/desert4.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/donuts1.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="desertCard">
                            <div class="cardWrapper">
                                <div class="card">
                                    <img src="@/assets/deserts/desert1.png" alt="desert">
                                </div>
                                <div class="cardDetails">
                                    <div class="cardTitle">
                                        <h2>Nazvanie tortika</h2>
                                    </div>
                                    <div class="cardButton">
                                        <button>Детільніше</button>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </swiper-slide>
                    <!-- <swiper-slide>Slide 2</swiper-slide>
                    <swiper-slide>Slide 3</swiper-slide>
                    <swiper-slide>Slide 4</swiper-slide>
                    <swiper-slide>Slide 5</swiper-slide>
                    <swiper-slide>Slide 6</swiper-slide>
                    <swiper-slide>Slide 7</swiper-slide>
                    <swiper-slide>Slide 8</swiper-slide>
                    <swiper-slide>Slide 9</swiper-slide> -->
                    <div class="swiperBtn">
                        <div ref="prevBtn" class="prevBtn sButton">
                            <img src="@/assets/arrowL.png" alt="arrowL">
                        </div>
                        <div ref="nextBtn" class="nextBtn sButton">
                            <img src="@/assets/arrowR.png" alt="arrowR">

                        </div>

                    </div>
                    
                </swiper>
              



            </div>
        </div>


    </div>
    

</template>

<script>
    import { ref } from 'vue';
    import { Swiper, SwiperSlide } from 'swiper/vue';

    // Import Swiper styles
    import 'swiper/css';

    import 'swiper/css/pagination';

    import '@/assets/style/main.scss';

    // import required modules
    import { Navigation, Pagination } from 'swiper/modules';

    export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        const prevBtn = ref(null);
        const nextBtn = ref(null);
        return {
        modules: [Pagination, Navigation],
        prevBtn,
        nextBtn,
        
        };
    },
    };

</script>

<style lang="scss">
.topDesertsBg{
    background-color: antiquewhite;
    .topDeserts{
        --mask:
            radial-gradient(49.31px at 50% 67.50px,#000 99%,#0000 101%) calc(50% - 50px) 0/100px 51% repeat-x,
            radial-gradient(49.31px at 50% -42.5px,#0000 99%,#000 101%) 50% 25px/100px calc(51% - 25px) repeat-x,
            radial-gradient(49.31px at 50% calc(100% - 67.50px),#000 99%,#0000 101%) calc(50% - 50px) 100%/100px 51% repeat-x,
            radial-gradient(49.31px at 50% calc(100% + 42.50px),#0000 99%,#000 101%) 50% calc(100% - 25px)/100px calc(51% - 25px) repeat-x;
        -webkit-mask: var(--mask);
                mask: var(--mask);
        background-color: rgb(48, 30, 6);
        width: 100vw;
        padding: 5vh 0;
        // height: 100vh;
        .container{
            .vector3{
                text-align: center;
                padding: 5vh 0 0 0;
                img{
                    filter: invert(1);
                    width: 50vw;
                }
            }
            .swiper{
                padding: 2vw;
                .swiper-slide {
                    text-align: center;
                    font-size: 18px;
                    background: antiquewhite;
                    border-radius: 2vw;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    height: initial;
                    width: 25vw;
                    overflow: hidden;
                    border: 5px solid teal;

                    .desertCard{
                        // display: inherit;
                        // justify-content: center;
                        // align-items: center;
                        width: -webkit-fill-available;
                        min-height: 50vh;

                        .cardWrapper{
                            .card{
                                display: flex;
                                justify-content: center;
                                position: relative;
                                img{
                                    position: relative;
                                    top: 0;
                                    transform: scale(1);
                                    transition: all ease 0.5s;
                                }
                            }
                            .cardDetails{
                                background-color: black;
                                position: absolute;
                                width: -webkit-fill-available;
                                height: -webkit-fill-available;
                                transition: all ease 0.5s;
                                padding: 3vh 0;
                                min-height: 30vh;
                                top: 40vh;
                                border-start-end-radius: 30%;
                                border-start-start-radius: 30%;
                                .cardTitle{
                                    color: white;

                                }
                                .cardButton{
                                    position: relative;
                                    top: 3vh;
                                }
                            }
                        }
                    }
                    
                }
                .swiper-slide:hover{
                    .desertCard{
                        .cardWrapper{
                            .card{
                                img{
                                    position: relative;
                                    transform: scale(1.8);
                                    transition: all ease 0.5s;
                                    top: 12vh;

                                }
                            }
                            .cardDetails{
                                background-color: rgb(48, 30, 6);
                                top: 35vh;
                                transition: all ease 0.5s;

                                .cardTitle{

                                }
                                .cardButton{
                                    
                                }
                            }
                        }
                    }
                }

                .swiper-slide img {
                    display: block;
                    max-width: 15vw;
                    height: inherit;
                    object-fit: cover;
                }
                .swiper-button-next::after{
                    content: none;
                }
                .swiper-button-prev::after{
                    content: none;
                }
                .swiperBtn{
                    display: flex;
                    justify-content: space-around;
                    margin-top: 5vh;
                    .sButton{
                        width: fit-content;
                        height: 5vh;
                        opacity: 1;
                        transition: all ease 0.5s;
                        background-color: antiquewhite;
                        border: 1px solid teal;
                        cursor: pointer;
                    }
                    .swiper-button-disabled{
                        opacity: 0.2;
                        transition: all ease 0.5s;
                        cursor: not-allowed;
                    }
                    img{
                        width: 7vw;
                    }
                }
            }
        }

    }

}
    

</style>