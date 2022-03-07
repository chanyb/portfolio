<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
        <p>
            튜닝의 끝은 순정..?!
        </p>
        <h3>Language</h3>
        <ul>
            <li><a href="" >Javascript</a></li>
            <li><a href="" >Python</a></li>
            <li><a href="" >JSP</a></li>
            <li><a href="" >HTML</a></li>
            <li><a href="" >CSS</a></li>
            <li><a href="" >Java</a></li>
            <li><a href="" >C, C++</a></li>
        </ul>
        <h3>Framework</h3>
        <ul>
            <li><a href="" >Vue.js</a></li>
            <li><a href="" >Nativescript</a></li>
            <li><a href="" >Bootstrap</a></li>
        </ul>
        <h3>Software</h3>
        <ul>
            <li><a href="" >Node.js</a></li>
            <li><a href="" >MySQL</a></li>
            <li><a href="" >Git</a></li>
            <li><a href="" >Jira</a></li>
        </ul>
        <h3>Service</h3>
        <ul>
            <li><a href="" >Progress - Kendo UI for vue</a></li>
            <li><a href="" >Progress - Kinvey</a></li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
