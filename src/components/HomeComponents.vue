<template>
<div>
        <h1 v-if="show">Hello from home components</h1>
        <h2 v-else>Changed</h2>
        <!-- <h2>{{data}}</h2> -->
        <!-- <button v-on:click="clickme('hello called')">clickme</button> -->
        <!-- <p v-if="show">this is for conditionally rendring </p>
        <p v-else>this is for conditionally else rendring </p> -->
        <button v-on:click="tap"> Toggle Button</button>

</div>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    // setup() {
        
    // },
    name: "HomeComponents",
    props: {
        data: String,
    },
    data(){
           return {show:true} 
    },
    methods: {
        tap()
        {
            this.show = !this.show
        }
    }
    
})
</script>
