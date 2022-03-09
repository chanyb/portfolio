<template>
    <div>
        <div class="row">
            <div class="col-md-12">
                <h1>{{ msg }}</h1>
            </div>
        </div>
        <div id="main">
            <div class="row">
                <div class="col-md-12">
                    <h3>Language</h3>
                </div>
            </div>
            <div>
                <div class="row" style="display:flex; justify-content: center;">
                    <div class="col-md-1">
                        <span class="item" @click="moveLeft()">Javascript</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">Python</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">JSP</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">HTML</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">CSS</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">Java</span>
                    </div>
                    <div class="col-md-1">
                        <span class="item">C, C++</span>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <h3>Framework</h3>
                </div>
            </div>
            <div class="row" style="display:flex; justify-content: center;">
                <div class="col-md-1">
                    <span class="item">Vue.js</span>
                </div>
                <div class="col-md-1">
                    <span class="item">Nativescript</span>
                </div>
                <div class="col-md-1">
                    <span class="item">Bootstrap</span>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <h3>Software</h3>
                </div>
            </div>
            <div class="row" style="display:flex; justify-content: center;">
                <div class="col-md-1">
                    <span class="item">Node.js</span>
                </div>
                <div class="col-md-1">
                    <span class="item">MySQL</span>
                </div>
                <div class="col-md-1">
                    <span class="item">Git</span>
                </div>
                <div class="col-md-1">
                    <span class="item">Jira</span>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <h3>Service</h3>
                </div>
            </div>
            <div class="row" style="display:flex; justify-content: center;">
                <div class="col-md-3">
                    <span class="item">Progress - Kendo UI for vue</span>
                </div>
                <div class="col-md-3">
                    <span class="item">Progress - Kinvey</span>
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
            console.log(mainFrame)
            mainFrame.classList.add('moveLeft')
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.item {
}
.item:hover {
    color: #238038;
    cursor: pointer;
}

@-webkit-keyframes moveLeft {
    from {
        background-color: 
    }
    to {
        background-color: yellow;
    }
}

.moveLeft {
    animation-name: moveLeft;
    animation-duration: 1s;
    animation-fill-mode: forwards;
}
</style>
