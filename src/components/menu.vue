<template>
    <div id="menu">
        <p class="tag" id="tag1">{{tag1}}</p>
        <p class="tag"  id="tag2">{{tag2}}</p>
        <p class="tag"  id="tag3">{{tag3}}</p>
        <p class="tag"  id="login">{{login}}</p>
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
        height: 50px;
        background-color: #6B6B6B;
        /*float: left;*/
    }

    .tag{
        height: 100%;
        width: 100px;
        margin-top: 0;
        margin-left: 40px;
        float: left;
        font-family: 'Open Sans', sans-serif;
        font-size: 20px;
        color: aqua;
        line-height: 50px;
    }

    #tag1{
        margin-left: 200px;
    }
    #login{
        float: right;
        width:200px;
    }
</style>