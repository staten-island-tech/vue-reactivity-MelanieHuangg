<template>
    <div class="cards">
        <h2 class="name">{{ Destination.name }}</h2>
        <img :src="Destination.img" alt="" class="img">
        <h3 class="description">{{ Destination.color }}</h3>
        <h3 class="description">${{ Destination.price }}.00</h3>
        <button id="btn" @click="addToCart()">Add To Cart</button>
    </div>
</template>

<script setup>
const props =defineProps({
    // age:Number,
    // name:String,
    Destination:Object,
});

//clicker logic 
const emit = defineEmits([
    "add"
])

function addToCart() {
    emit("add")
}



</script>

<style scoped> 
/* scoped means no other object will be effected */

img{
    width:250px;
    height:300px;
    object-fit:cover;
    
}

.cards{
   display: flex;
   flex-direction: column;
   align-items: center;
   border: solid black;
   padding: 3%;
   background-color: rgb(195, 191, 177);
   width:400px;
   margin: 1%;
   border-radius: 1rem;

}

.name{
    text-align: center;
    font-family: "Dosis", sans-serif;
}

.img{
    border: solid black ;
    border-radius: 1rem;
}

.description{
    text-align: center;
    font-family: "Dosis", sans-serif;
}

#btn{
    text-align: center;
    margin-top: 1rem;
    border-radius: 1rem;
    font-family: "Dosis", sans-serif;
    padding: 4%;
    padding-left: 6%;
    padding-right: 6%;
}

#btn:hover{
    opacity: 0.7;
    cursor: pointer;
    transition: all 0.2s;
    box-shadow: 0 10px 0.5rem rgba(0, 0, 0, 0.2);
}


</style>