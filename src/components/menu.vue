<template>
    <div id="menu">
        <a class="tag tag1" >{{tag1}}</a>
        <a class="tag tag2" >{{tag2}}</a>
        <a class="tag tag3" >{{tag3}}</a>
        <a class="tag login" >{{login}}</a>
    </div>
</template>

<script>
    export default {
        name: "topmenu",
        data(){
            return{
                tag1:"Blogs",
                tag2:"Projects",
                tag3:"Contact",
                login:"Login or Signin"
            }
        }
    }
</script>

<style scoped>
    #menu{
        position: fixed;
        top:0;
        left: 0;
        right: 0;
        margin: 0;
        width: 100%;
        min-width: 600px;
        height: 50px;
        background-color: #6B6B6B;
        /*float: left;*/
    }

    #menu a:hover{
        background-color: #707070;
        cursor: pointer;
    }

    .tag{
        height: 100%;
        width: 100px;
        margin: 0;
        /*margin-left: 40px;*/
        float: left;
        font-family: 'Open Sans', sans-serif;
        font-size: 20px;
        color: aqua;
        line-height: 50px;
    }

    .tag1{
        margin-left: 100px;
    }
    .tag2{
        margin-left: 0px;
    }
    .tag3{
        margin-left: 0;
    }
    .login{
        float: right;
        width:200px;
    }
</style>