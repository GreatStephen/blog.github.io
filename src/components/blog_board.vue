<template>
    <div id="blog_board">
<!--        blog board-->
        <blogs
            v-for="s in str"
            v-bind:key="s['id']"
            v-bind:userId="s['userId']"
            v-bind:id="s['id']"
            v-bind:title="s['title']"
            v-bind:body="s['body']">
        </blogs>
    </div>
</template>

<script>
    import blogs from "./blogs";

    export default {
        name: "blog_board",
        components: {
            blogs
        },
        data:function(){
            return {
                str: "message",
            }
        },
        created() {
            let URL = "https://jsonplaceholder.typicode.com/POSTS";
            let request = new XMLHttpRequest();
            let self = this;
            let load = function(){
                let responseText = request.response;
                let datas = JSON.parse(responseText);
                self.str=datas;
                // console.log(self.str);
                self.createBlog();
            };

            request.open('GET', URL );
            request.responseType='text';
            request.send();
            request.onload = load;

        },

        methods: {
            createBlog(){
                console.log(this.str);

            }
        }
    }

</script>

<style scoped>
    #blog_board{
        width: 100%;
        height: 100%;
        /*background-color: azure;*/
        z-index: 0;
        margin: 0 auto;
        color:black;
        text-align: center;
    }
</style>