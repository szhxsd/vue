<template>
<div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <!-- <h1>{{ title }}</h1> -->

    <h1 v-html="title" v-on:click='toggleFinish("hxsd")'></h1>


</div>
</template>

<script>

export default {
    //name: 'app',

     data:function(){
        return {
          //msg: 'Welcome to Your Vue.js App'
          title:"<span>?</span>我是一条标题"
        }
    },

    // data() {
    //     return {
    //         msg: '扔出一条信息'
    //     }
    // },

    // components: {
    //     Hello
    // }

    methods:{
        toggleFinish:function(a){
            console.log(a)
        }
    }
}
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}

h1,
h2 {
    font-weight: normal;
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
