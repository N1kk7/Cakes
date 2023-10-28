<template>
    <div class="Author"> 
        <div class="authorSweets">
            <div class="container">
                <div class="line">
                    <img src="@/assets/border2.png" alt="img">
                </div>
                <div class="componentTitle">
                    <h1>АВТОРСЬКІ ТОРТИ, ДЕСЕРТИ, ТА СОЛОДОЩІ РУЧНОЇ РОБОТИ</h1>
                </div>
                <div class="vector">
                    <img src="@/assets/vector1.png" alt="vector">
                </div>
                <div class="authorItem">
                    <div class="item ">
                        <img src="@/assets/authorSweets/author1.png" alt="author">
                    </div>
                    <div class="itemDescription">
                        <h4>Кондитерські вироби будь якої складності з дбайливою доставкою</h4>

                    </div>
                    <div class="item iLeft">
                        <img class="itemCake" src="@/assets/authorSweets/author2.jpg" alt="author">
                    </div>
                    
                </div>
                <div class="roundButton">
                    <div class="roundWrapper">
                        <h1>КАТАЛОГ</h1>
                        <h2>-></h2>
                    </div>
                   
                </div>

            </div>
        </div>
       


    </div>
</template>

<script>    
</script>

<style lang="scss">
    .Author{
        height: 105vh;

        .authorSweets{
        width: 100vw;
        background-color: antiquewhite;
        position: relative;
        bottom: 5vh;

        .container{

            .line{
                text-align: center;
                padding: 5vh 0  2vh 0;
                img{
                    width: 40vw;
                }

            }
            // .componentTitle{   //!!!!!!!!! ALLL STYLES
            //     text-align: center;
            //     h1{
            //         color: rgb(99, 99, 99);
            //         font-size: 4vw;
            //         letter-spacing: 0.5vw;
            //     }
            // }
            .authorItem{
                display: flex;  
                justify-content: space-around;
                align-items: center;
                position: relative;
                .item{
                    border: 1px solid black;
                    transform: rotateZ(-20deg);
                    display: inherit;
                    align-items: center;
                    justify-content: center;
                    border-radius: 50%;
                    width: 40vh;
                    height: 60vh;
                    img{
                        width: 25vw;
                        padding: 2vh;
                    }
                    .itemCake{
                        width: 30vw;
                    }
                    
                    
                }
                .itemDescription{
                    position: absolute;
                    top: 5vh;
                    font-size: 1.5vw;
                    width: 30vw;
                }
                .iLeft{
                    transform: rotateZ(-5deg);
                    background-color: rgb(80, 51, 14);
                    flex-direction: column;
                    width: 50vh;
                    height: 40vh;
                    img{
                        width: 35vw !important;
                        border-radius: 2vw;
                        filter: brightness(0.75);
                        border: 1px solid white;
                        padding: unset;
                    }

                }

            }
            .roundButton{
                text-align: center;
                display: flex;
                justify-content: center;
                position: relative;
                bottom: 16vh;
                .roundWrapper{
                    background-color: burlywood;
                    width: 180px;
                    height: 180px;
                    border-radius: 50%;
                    display: inherit;
                    flex-direction: column;
                    justify-content: center;
                    border: 1px solid rgb(99, 99, 99);
                  


                    h1{
                        color: rgb(99, 99, 99);
                        font-size: 1.5vw;
                        letter-spacing: 0.5vw;
                    }
                    h2{
                        color: rgb(99, 99, 99);
                    }

                    
                }

                .roundWrapper:hover{
                    border: 2px solid white;
                    background-color: rgb(48, 30, 6);
                    cursor: pointer;
                    h1{
                        color: white;

                    }
                    h2{
                        color: white;
                    }
                }
                    

                
                
               
            }
            

        }
    }
    }

</style>