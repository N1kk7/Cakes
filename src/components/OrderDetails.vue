<template>
    <div class="orderDetailsBg">
        <div class="orderDetails">
            <div class="container">
                <div class="vector3">
                    <img src="@/assets/vector3.png" alt="vector3">
                </div>
                <div class="componentTitle titleBlack">
                    <h1>Як ми працюємо?</h1>
                </div>
                <div class="vector vectorDark">
                    <img src="@/assets/vector1.png" alt="vector">
                </div>
                <div class="listDetails">
                    <ul>
                        <li>
                            <div class="itemTitle">
                                <h1>ЗАМОВЛЕННЯ</h1>
                            </div>
                        </li>
                        <li>
                            <div class="itemTitle">
                                <h1>ДЕТАЛІ</h1>
                            </div>
                        </li>
                        <li>
                            <div class="itemTitle">
                                <h1>ПРОЦЕСС</h1>
                            </div>
                        </li>
                        <li>
                            <div class="itemTitle">
                                <h1>ДОСТАВКА</h1>
                            </div>
                        </li>

                    </ul>
                </div>
                <hr>
                <div class="orderDescription">
                    <div class="imgDescription">
                        <img src="@/assets/orderCake.jpg" alt="orderCake">
                    </div>
                    <div class="textDescription">
                        <ul>
                            <li>
                                <p>
                                    Додайте товар до корзини, виберіть кількість, начинку. Залиште свої контактні данні та вкажіть деталі замовлення!
                                </p>
                            </li>
                            <li>
                                <p>
                                    Після отримання замовлення наш оператор звʼяжется з вами найближчим часом для уточнення деталей замовлення!
                                </p>
                            </li>
                            <li>
                                <p>
                                    Ми виконаємо замовлення в поставлений термін, дбайливо запакуємо та підготовимо замовлення до видачі!
                                </p>
                            </li>
                            <li>
                                <p>
                                    Наші курьери доставлять замовлення до Вашого свята. Також є можливість самостійного отримання замовлення!
                                </p>
                            </li>

                        </ul>
                    </div>
                    <div class="button">
                            <button href="#" @click="() => scrollTo('#form')">Замовити</button>
                    </div>
                    <!-- function () {console.log('log')} -->
                </div>
                
            </div>
        </div>

    </div>
</template>

<script>

</script>


<style lang="scss">
    .orderDetailsBg{
        background-color: antiquewhite;
        .orderDetails{
        --mask:
            radial-gradient(49.31px at 50% 67.50px,#000 99%,#0000 101%) calc(50% - 50px) 0/100px 51% repeat-x,
            radial-gradient(49.31px at 50% -42.5px,#0000 99%,#000 101%) 50% 25px/100px calc(51% - 25px) repeat-x,
            radial-gradient(49.31px at 50% calc(100% - 67.50px),#000 99%,#0000 101%) calc(50% - 50px) 100%/100px 51% repeat-x,
            radial-gradient(49.31px at 50% calc(100% + 42.50px),#0000 99%,#000 101%) 50% calc(100% - 25px)/100px calc(51% - 25px) repeat-x;
        -webkit-mask: var(--mask);
                mask: var(--mask);
        background-color: rgb(48, 30, 6);
        min-height: 100vh;
        // padding: 0 0 5vh 0;


        .vector3{
                text-align: center;
                padding: 5vh 0 0 0;
                img{
                    filter: invert(1);
                    width: 50vw;
                }
            }
        
        }
        .listDetails{
            text-align: center;
            padding: 2vh 0;
            ul{
                li{
                    display: inline-block;
                    list-style-type: none;
                    width: 23vw;
                    padding: 0 1vw;
                    .itemTitle{
                        color: white;
                    }
                }
            }
        }
        .orderDescription{
            text-align: center;
            position: relative;
            padding: 2vh 0;
            .imgDescription{
                img{
                    width: 90vw;
                    height: 55vh;
                    object-fit: cover;
            }
                
            }
            .textDescription{
                position: absolute;
                width: 100vw;
                top: 5vh;
                ul{
                    display: flex;
                    align-items: stretch;
                    justify-content: center;
                    text-align: center;
                    padding: 0;
                    li{
                        display: inline-block;
                        background-color: rgba(0, 0, 0, 0.7);
                        list-style-type: none;
                        border: 1px solid white;
                        text-align: start;
                        min-height: 20vh;
                        padding: 1vw;
                        margin: 0 1vw;
                        width: 22vw;

                        p{
                            color: white;
                            width: 20vw;
                            font-size: 1.5vw;
                        }
                    }
                }
            }
            .button{
                width: 20%;
                height: 5vh;
                position: relative;
                bottom: 10vh;
                margin: 0 auto;
                cursor: pointer;
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
    


</style>