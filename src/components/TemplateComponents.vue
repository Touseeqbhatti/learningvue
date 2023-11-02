<template>
    <div>
<h1 >Template components</h1>
<h1 >{{name}}</h1>
<h3 >{{ok?"yes":"no"}}</h3>
<button v-on:click="change">Button to change</button>
    </div>
</template>
<script>
export default {
    name:"TemplateComponents",
    data(){
        return {show:false,
        name:"ali"+" "+ (10+20),
        ok:true,
        }    

    },
    methods:{
        change(){
            this.ok= !this.ok
        }
    }

}
</script>