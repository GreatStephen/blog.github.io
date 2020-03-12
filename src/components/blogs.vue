<template>
    <div id="blogs">
        <div  id="user_icon">
            <img src="../assets/user.png">
            <h2>user{{userId}}</h2>
        </div>
        <h1>{{title}}</h1>
        <div id="blog-content">
            <img src="http://www.wpthemegenerator.com/wp-content/uploads/2012/06/Image.jpg">
            <p>{{body}}</p>
        </div>
        <br />

    </div>
</template>

<script>
    export default {
        name: "blogs",
        props:['userId', 'id', 'title', 'body']
    }
</script>

<style scoped>
    #blogs {
        background: #fff;
        margin: 20px auto;
        display: block;
        width: 50%;
        height: 100%;
        padding:20px;
        border-radius: 2px 2px 2px 2px;
        -webkit-box-shadow: 0 1px 4px
        rgba(0, 0, 0, 0.3), 0 0 40px
        rgba(0, 0, 0, 0.1) inset;
        -moz-box-shadow: 0 1px 4px rgba(0, 0, 0, 0.3), 0 0 40px rgba(0, 0, 0, 0.1) inset;
        box-shadow: 0 1px 4px
        rgba(0, 0, 0, 0.3), 0 0 40px
        rgba(0, 0, 0, 0.1) inset;
    }

    /*#blogs img {*/

    /*    width: 75%;*/
    /*    margin-top: 15px;*/
    /*}*/

    #user_icon{
        width: 100%;
        height: 50px;
    }

    #user_icon img{
        float: left;
        margin-left: 0;
        margin-top: 1%;
        width: 5%;
    }

    #user_icon h2{
        float: right;
        margin-right: 85%;
        width: 10%;
    }

    #blog-content{
        width: 100%;
        height: 200px;
        margin-top: 50px;
    }
    #blog-content img{
        height: 75%;
        /*width: 50%;*/
        float: left;
        margin-left: 0;
    }
    #blog-content p{
        float: right;
        margin-right: 0;
        width: 50%;
        font-size: 20px;
        font-family: "Times New Roman";
    }

    p{
        margin-top: 15px;
        text-align: justify;
    }

    h1{
        font-size: 25px;
        font-weight: bold;
        margin-top: 5px;
        text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
    }

    a{
        text-decoration: none;
        color: #4A4A4A !important;
    }

    a:hover{
        text-decoration: underline;
        color: #6B6B6B !important ;
    }

</style>