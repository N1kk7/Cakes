<template>
    <div>
        <div class="fillings">
            <div class="container">
                <div class="line">
                    <img src="@/assets/border2.png" alt="vector">
                </div>
                <div class="componentTitle">
                    <h1>Ми пропонуємо наступні начинки</h1>
                </div>
                <div class="vector">
                    <img src="@/assets/vector1.png" alt="vector">
                </div>
                <div class="fillingsItem">
                    <ul>
                        <li>
                            <div class="cardImg">
                                <img src="@/assets/fillings/medovik.png" alt="medovik">
                            </div>
                            <div class="cardName">
                                <h2>Медовик</h2>
                            </div>

                        </li>
                        <li>
                            <div class="cardImg">
                                <img src="@/assets/fillings/barhat.png" alt="barhat">
                            </div>
                            <div class="cardName">
                                <h2>Бархат</h2>
                            </div>
                        </li>
                        <li>
                            <div class="cardImg">
                                <img src="@/assets/fillings/snickers.png" alt="snickers">
                            </div>
                            <div class="cardName">
                                <h2>Snickers</h2>
                            </div>
                        </li>
                        <li>
                            <div class="cardImg">
                                <img src="@/assets/fillings/cherry.png" alt="cherry">
                            </div>
                            <div class="cardName">
                                <h2>Cherry</h2>
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="vectorCake">
                    <img src="@/assets/vectorCake.png" alt="vectorCake">
                </div>

            </div>

        </div>
    </div>
    

</template>


<script>


</script>


<style lang="scss">
    .fillings{
        background-color: antiquewhite;
        // .line{
        //     text-align: center;
        //     img{             !!!! remove all lines from project
        //         width: 40vw;
        //     }
        // }
        .fillingsItem{
            ul{
                padding: 0;
                text-align: center;
                li{
                    position: relative;
                    display: inline-block;
                    margin: 2vw 1vw;
                    .cardImg{
                        img{
                        width: 20vw;
                        filter: brightness(0.75);
                        }
                    }
                    .cardName{
                        position: absolute;
                        bottom: 0.7vh;
                        h2{
                            color: white;
                            background-color: rgba(0, 0, 0, 0.4);
                            padding: 1vh 2vh;
                        }
                    }
                    
                }
            }
        }
        .vectorCake{
            text-align: center;
            padding: 2vh 0;
            img{
                width: 15vw;
            }
        }
    }

    





</style>