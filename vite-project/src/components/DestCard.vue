<template>
    <div>
        <h2>{{ Destination.name }}</h2>
        <img :src="Destination.img" alt="">
        <h3>{{ Clicked }}</h3>
        <button @click="increment">Click Me</button>
    </div>
</template>

<script setup>
import {ref} from "vue";
const props =defineProps({
    // age:Number,
    // name:String,
    Destination:Object,
});

//clicker logic 
const clicked = ref(0); 
function increment(){
    clicked.value++; //will increase the number 0 by increments of 1 
}
</script>

<style scoped> 
/* scoped means no other object will be effected */

img{
    width:250px;
    height:300px;
    object-fit:cover;
}

</style>