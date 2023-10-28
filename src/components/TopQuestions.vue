<template>
    <div class="topQuestionBg">
        <div class="topQuestion">
            <div class="container">
                <div class="line">
                    <img src="@/assets/border2.png" alt="vector">
                </div>
                <div class="componentTitle">
                    <h1>
                        Найбільш поширені питання
                    </h1>
                </div>
                <div class="vector">
                    <img src="@/assets/vector1.png" alt="vector">
                </div>

                <div class="questionsBlock">
                    <div class="questions">
                        <ul>
                        <li>
                            <div class="question" @click="questionClick('question1')">
                                <h4>
                                    Як оплатити замовлення?
                                </h4>
                            </div>
                        </li>
                        <li>
                            <div class="question" @click="questionClick('question2')">
                                <h4>
                                    Як розрахувати вагу торту?
                                    
                                </h4>
                            </div>
                        </li>
                        <li>
                            <div class="question" @click="questionClick('question3')">
                                <h4>
                                    Який термін зберігання ваших тортів та десертів?
                                </h4>
                            </div>
                        </li>
                        <li>
                            <div class="question" @click="questionClick('question4')">
                                <h4>
                                    Який термін виготовлення торту?
                                    
                                </h4>
                            </div>
                        </li>
                        <li>
                            <div class="question" @click="questionClick('question5')">
                                <h4>
                                    Ви можете виготовити торт по моєму дизайну?
                                    
                                </h4>
                            </div>
                        </li>
                        <li>
                            <div class="question" @click="questionClick('question6')">
                                <h4>
                                    На яку знижку я можу розраховувати?
                                    
                                </h4>
                            </div>
                        </li>

                    </ul>
                    </div>
                    <div class="answerBlock">
                        <img src="@/assets/topQuestion.png" alt="">
                        <div class="answers">
                            <div class="answer " :class="{answer1}">
                                <div class="closeBtn" @click="closeAnswer">
                                    <span>close</span>
                                </div>
                                <p>
                                    1  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div>
                            <div class="answer" :class="{answer2}" >
                                <div class="closeBtn" @click="closeAnswer">
                                    <span>close</span>
                                </div>
                                <p>
                                    2  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div><div class="answer" :class="{answer3}">
                                <div class="closeBtn" @click="closeAnswer">
                                    <span>close</span>
                                </div>
                                <p>
                                    3  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div><div class="answer" :class="{answer4}">
                                <div class="closeBtn" @click="closeAnswer">
                                    <span>close</span>
                                </div>
                                <p>
                                    4  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div><div class="answer" :class="{answer5}">
                                <div class="closeBtn" @click="closeAnswer"> 
                                    <span>close</span>
                                </div>
                                <p>
                                    5  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div><div class="answer" :class="{answer6}">
                                <div class="closeBtn" @click="closeAnswer">
                                    <span>close</span>
                                </div>
                                <p>
                                    6  Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores odit iste obcaecati nam sint numquam molestiae suscipit excepturi maxime voluptas eaque pariatur omnis nisi, sapiente sit cum repudiandae porro quam.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>


            </div>

        </div>

    </div>
    
</template>


<script>

    export default{
        data() {
            return{
                answer1: '',
                answer2: '',
                answer3: '',
                answer4: '',
                answer5: '',
                answer6: '',

            }



        },
        methods:{
            questionClick  (q) {
                // console.log(q);
                q === 'question1' ? this.answer1 = q : this.answer1 = '';
                q === 'question2' ? this.answer2 = q : this.answer2 = '';
                q === 'question3' ? this.answer3 = q : this.answer3 = '';
                q === 'question4' ? this.answer4 = q : this.answer4 = '';
                q === 'question5' ? this.answer5 = q : this.answer5 = '';
                q === 'question6' ? this.answer6 = q : this.answer6 = '';


                // answerClass = q;
                // console.log(q);
            },
            closeAnswer(){
                this.answer1 = '';
                this.answer2 = '';
                this.answer3 = '';
                this.answer4 = '';
                this.answer5 = '';
                this.answer6 = '';
            }

        },
    }


</script>

<style lang="scss">
    .topQuestionBg{
        background-color: antiquewhite;
        min-height: 100vh;
        padding-bottom: 5vh;
       .topQuestion{
            .container{

                .questionsBlock{
                    text-align: center;
                    // background-color: rgba(0,0,0,0.5);
                    width: 90vw;
                    border: 1px solid rgb(48, 30, 6);
                    margin: 5vh auto 0;

                    .questions{
                        ul{
                            padding: 0;
                            text-align: center;
                            li{
                                display: inline-block;
                                cursor: pointer;
                                text-align: justify;
                                width: 40vw;
                                height: 5vh;
                                border-bottom: 1px solid gray;
                                margin: 2vw;
                                h4{
                                    // height: 2vh;
                                    font-size: 1.5vw;
                                    padding: 10px 1vw; 
                                    color: gray;
                                }


                            }
                            li:hover{
                                h4{
                                    background-color: rgb(48, 30, 6);
                                    color: antiquewhite;


                                }
                            }
                        }

                    }
                    .answerBlock{
                        position: relative;
                        img{
                            width: 80vw;
                            // filter: brightness(0.7);
                        }
                        .answers{
                            .answer{
                                display: none;
                                transition: all ease 0.5s;
                                .closeBtn{
                                    position: absolute;
                                    top: 0;
                                    right: 0;
                                    border: 1px solid antiquewhite;
                                    padding: 5px;
                                    cursor: pointer;
                                }
                            }
                            .answer1, .answer2, .answer3, .answer4, .answer5, .answer6{
                                display: block;
                                position: absolute;
                                transition: all ease 0.5s;
                                top: 0;
                                z-index: 5;
                                color: antiquewhite;
                                font-size: 2vw;
                                border: 1px solid antiquewhite;
                                margin: 8vw;
                                background-color: rgba(0,0,0,0.5);
                                padding: 5vh;
                            }
                        }
                    }
                    
                }
            }
       }
    }


</style>