<template>
    <div>
        <table border="1px">
            <tr>
                <td>ID</td>
                <td>Email</td>
                <td>Name</td>
            </tr>
            <tr v-for="user in users" :key="user.id">
                <td>{{user.id}}</td>
                <td>{{user.email}}</td>
                <td>{{user.name}}</td>
            </tr>
        </table>
    </div>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    // setup() {
        
    // },
    name: "ForLoopComponents",
    data(){
        return {
            users:[
            {id:1,name:"touseeq",email:"touseeq@gmail.com"},
            {id:2,name:"ali",email:"ali@gmail.com"},
            {id:3,name:"bkr",email:"bkr@gmail.com"},
            {id:4,name:"ahmad",email:"ahmad@gmail.com"},
        ]
        }
    }
})
</script>
