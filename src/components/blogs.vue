<template>
    <div id="blogs">
        <div  id="user_icon">
            <img src="../assets/user.png">
            <h2>user{{userId}}</h2>
        </div>
<!--        <h1>{{title}}</h1>-->
<!--        <div id="blog-content">-->
<!--            <img src="http://www.wpthemegenerator.com/wp-content/uploads/2012/06/Image.jpg">-->
<!--            <p>{{body}}</p>-->
<!--        </div>-->
        <div id="blog-title">
            <div id="img-wrapper">
                <img src="http://www.wpthemegenerator.com/wp-content/uploads/2012/06/Image.jpg">
            </div>
            <a>{{title}}</a>
        </div>

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
        min-width: 600px;
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
        height: 40px;
        cursor: default;
    }

    #user_icon img{
        float: left;
        margin: 0;
        width: 40px;
        height: 40px;
    }

    #user_icon h2{
        float: left;
        margin: auto ;
        line-height: 40px;
        width: 10%;
    }

    #blog-title{
        width: 100%;
        height: 100px;
        margin: 20px auto;
    }
    #img-wrapper{
        width: 200px;
        height: 100px;
        float: left;
    }
    #img-wrapper img{
        height: 100%;
        width: 100%;
        float: left;
        margin-left: 0;
    }
    #blog-title a{
        width: calc(100% - 220px);
        height: 100%;
        margin: 5px 10px;
        float: right;
        font-size: 25px;
        font-weight: bold;
        text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
        font-family: "Times New Roman";
        text-align: left;
        text-decoration: none;
        color: #4A4A4A !important;
    }

    #blog-title a:hover{
        text-decoration: underline;
        color: #6B6B6B !important ;
        cursor: pointer;
    }


    /*a{*/
    /*    text-decoration: none;*/
    /*    color: #4A4A4A !important;*/
    /*}*/

    /*a:hover{*/
    /*    text-decoration: underline;*/
    /*    color: #6B6B6B !important ;*/
    /*}*/

</style>