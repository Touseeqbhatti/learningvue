<template>
    <div>
<h1 style="white-space:pre-line">{{msg}}</h1>
<textarea  v-model="msg"/>
    </div>
</template>

<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    name: 'DataBinding',
    data(){
        return {
            msg: "hi"
        }
    }
})
</script>
