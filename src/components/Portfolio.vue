<template>
    <div class="portfolio">
        <div class="projects">
            <a href="https://babzshop.netlify.app">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/e-commerce.png" alt="">
                    </div>
                    <p class="click">Click to view my e-commerce website.</p>
                </div>
            </a>
            <a href="https://babzbank.netlify.app">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/hoobank.png" alt="">
                    </div>
                    <p class="click">Visit Hoobank with a tap.</p>
                </div>
            </a>
            <a href="https://babz-cinema.netlify.app">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/movieapp.png" alt="">
                    </div>
                    <p class="click">Click to stream movies.</p>
                </div>
            </a>
            <a href="https://babzt.github.io/iPhone13/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/iphone.png" alt="">
                    </div>
                    <p class="click">Click to view an iPhone I built.</p>
                </div>
            </a>
            <a href="https://babzt.github.io/myStore/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/ecommerce2.png" alt="">
                    </div>
                    <p class="click">Click Me.</p>
                </div>
            </a>
            <a href="https://foodchannel.netlify.app">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/foodchannel.png" alt="">
                    </div>
                    <p class="click">Visit my food channel.</p>
                </div>
            </a>
        </div>

        <div v-if="otherProjects" class="other_work">
            <a href="https://babzt.github.io/Cowrywise/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/cowrywise.png" alt="">
                    </div>
                    <p class="click">Tap to view Cowrywise Landing page clone.</p>
                </div>
            </a>
            <a href="https://babzt.github.io/PiggyvestHomePage/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/piggyvest.png" alt="">
                    </div>
                    <p class="click">Tap to view PiggyVest Landing page clone.</p>
                </div>
            </a>
            <a href="https://babzt.github.io/QuizApp/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/quiz.png" alt="">
                    </div>
                    <p class="click">Click to take Quiz.</p>
                </div>
            </a>
            <a href="https://babzt.github.io/GigPrix/">
                <div class="work">
                    <div class="imagediv">
                        <img src="@/assets/gigprix.png" alt="">
                    </div>
                    <p class="click">Click Me</p>
                </div>
            </a>
        </div>

        <div class="load_more" @click="loadMoreProjects">
            <button v-if="otherProjects">View less</button>
            <button v-else>Load More Projects</button>
            
        </div>
    </div>
</template>

<script>
    export default {
        name:'PortfolioComp',
        data(){
            return{
                otherProjects:false
            }
        },
        methods:{
            loadMoreProjects(){
                this.otherProjects = !this.otherProjects;
            }
        }
    }
</script>
