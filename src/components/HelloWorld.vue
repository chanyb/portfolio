<template>
    <div>
        <div class="row">
            <div class="col-md-12">
                <h1>{{ msg }}</h1>
            </div>
        </div>
        <div class="row">
            <div id='skillBody' class="col-md-12">
                <div>
                    <h3>Language</h3>
                </div>
                <div class="row">
                    <span class="item" @click="toggleItem('javascript')">Javascript</span>
                    <span class="item" @click="toggleItem('python')">Python</span>
                    <span class="item" @click="toggleItem('jsp')">JSP</span>
                    <span class="item preparing">HTML</span>
                    <span class="item preparing">CSS</span>
                    <span class="item preparing">Java</span>
                    <span class="item preparing">C, C++</span>
                </div>
                <div class="row">
                    <h3>Frameworks</h3>
                </div>
                <div class="row">
                    <span class="item preparing">Vue.js</span>
                    <span class="item preparing">Nativescript</span>
                    <span class="item preparing">Bootstrap</span>
                </div>
                <div class="row">
                    <h3>Software</h3>
                </div>
                <div class="row">
                    <span class="item preparing">Node.js</span>
                    <span class="item preparing">MySQL</span>
                    <span class="item" @click="toggleItem('git')">Git</span>
                    <span class="item preparing">Jira</span>
                </div>
                <div class="row">
                    <h3>Service</h3>
                </div>
                <div class="row">
                    <span class="item preparing">Progress - Kendo UI for vue</span>
                    <span class="item preparing">Progress - Kinvey</span>
                </div>
            </div>
            <div v-if="flag.itemToggle" class="col-md-6 window-mr">
                <div class="row" id="javascript" v-if="flag.itemToggle==='javascript'">
                    <div class="col-md-12">
                        <img src="@/assets/metory_1.png" style="width:100%; border: 1px solid black;" />
                    </div>
                    <div class="col-md-12">
                        <!-- description -->
                        <p>블록체인 기반 임상연구 플랫폼</p>
                        <ul style="text-align: left;">
                            <li>frontend, backend 작성에 javascript를 기반으로하는 프레임워크인 vue.js, node.js를 활용했습니다.</li>
                            <li>비동기/동기 처리와 ES6문법(() => {}, ${}, [...arr, obj] 등..)에 대한 이해가 있습니다.</li>
                        </ul>
                    </div>
                </div>
                <div class="row" id="python" v-if="flag.itemToggle==='python'">
                    <div class="col-md-12">
                        <img src="@/assets/python_1.png" style="width:100%; border: 1px solid black;" />
                    </div>
                    <div class="col-md-12">
                        <!-- description -->
                        <p>오토인코더를 통한 iris data manifold 확인</p>
                        <ul style="text-align: left;">
                            <li>tensorflow를 활용해 신경망 모델을 설계할 수 있습니다.</li>
                            <li>파이썬의 문법을 이해하고 있으며, Selenium을 이용해 동적 크롤링을 하는 등의 작업이 가능합니다.</li>
                        </ul>
                    </div>
                </div>
                <div class="row" id="jsp" v-if="flag.itemToggle==='jsp'">
                    <div class="col-md-12">
                        <img src="@/assets/jsp_1.png" style="width:100%; border: 1px solid black;" />
                    </div>
                    <div class="col-md-12">
                        <!-- description -->
                        <p>블록체인 기반 임상연구 플랫폼</p>
                        <ul style="text-align: left;">
                            <li>JSP를 사용해 세션에 값을 저장하고 유저의 인증 등의 Backend 개발을 할 수 있습니다.</li>
                        </ul>
                    </div>
                </div>
                <div class="row" id="git" v-if="flag.itemToggle==='git'">
                    <div class="col-md-12">
                        <img src="@/assets/git_1.png" style="width:100%; border: 1px solid black;" />
                    </div>
                    <div class="col-md-12">
                        <!-- description -->
                        <p>https://github.com/chanyb</p>
                        <ul style="text-align: left;">
                            <li>git을 이용한 버전 관리, 협업이 가능합니다.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HelloWorld',
    props: {
        msg: String
    },
    methods: {
        moveLeft: function() {
            var mainFrame = document.getElementById('main')
            mainFrame.classList.add('moveLeft')
        },
        toggleItem: function(val) {
            var skillBody = document.getElementById('skillBody')

            var targetClass = skillBody.classList
            
            if (targetClass.length === 1) {
                skillBody.classList.add('col-md-6')
                skillBody.classList.add('moveLeft')
                skillBody.classList.remove('col-md-12')

                skillBody.addEventListener("animationend", () => {
                    this.flag.itemToggle = val
                }, false)
            }
            else {
                this.flag.itemToggle = val
            }
        }
    },
    data() {
        return {
            flag: {
                itemToggle: false
            },
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.item {
    margin-right: 10px;
}
.item:hover {
    color: #238038;
    cursor: pointer;
}
.preparing {
    color: gray;
}
.preparing:hover {
    color: gray;
    cursor: default;
}

@-webkit-keyframes moveLeft {
    from {
        left:30vh;
    }
    to {
        left:0px;
    }
}

.moveLeft {
    animation-name: moveLeft;
    animation-duration: 1s;
    animation-fill-mode: forwards;
}

@media all and (min-width: 1200px) {
    .window-mr {
        padding-right: 10%
    }
}
</style>
s