<template>
    <div>
<p v-html="rowHtml"></p>
<h1 v-bind:style="{color:'red'}">{{name}}</h1>
<h3 class="h3class">{{ok?"yes":"no"}}</h3>
<button v-bind:disabled="disablebtn" v-on:click="change">Button to change</button>
<h1 v-bind:class="{display: show1}">This is conditional class </h1>
<h1 v-bind:class="[show?aclass:display]">This is array class </h1>
    </div>
</template>
<script>
export default {
    name:"TemplateComponents",
    data(){
        return {show:false,
        name:"ali"+" "+ (10+20),
        ok:true,
        rowHtml: "<h1 >Template components</h1>",
        show1: true,
        aclass:'arrayclass',
        }    

    },
    methods:{
        change(){
            this.ok= !this.ok
            }
    }

}
</script>
<style scoped>
.h3class{
    color: blue;
}
.display{
    background-color: brown;
}
.arrayclass{
    background-color: red;
}
</style>