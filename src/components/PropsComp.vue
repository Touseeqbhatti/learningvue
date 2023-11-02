<template>
    <div>
<!-- <h1>{{name}}</h1> -->
<h1 v-for="user in name" :key="user.name">{{user.name}}--{{user.email}}</h1>
    </div>
</template>

<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    name: 'PropsComp',
    props:[
        'name'
    ]
})
</script>
