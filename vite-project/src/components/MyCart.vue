<template>
    <div class="cart">
        <h2 class="cartTitle">Cart:</h2>
        <div 
        v-for="destination in props.cart" 
        :key="destination.name"
        class="cartInfo"
        >
            <h2>{{ destination.name }}</h2>
            <h3>{{ destination.color }}</h3>
            <h3>${{ destination.price }}.00</h3>
        </div>
        <div>
            <h2 class="total"> Total = ${{ props.total }}.00</h2>
        </div>
      
    </div>
</template>

<script setup>
//props are the specific things you want to pass to the component (ex: the name and price)
import { defineProps } from "vue";

const props = defineProps({ cart: Array, total: Number })


</script>

<style scoped>

.cartInfo{
    color: black;
    width: 17rem;
    margin-bottom: 1%;
    border: solid black;
    background-color: rgb(195, 191, 177);
    padding-inline-start: 1%;
    border-radius: 1rem;
    font-family: "Dosis", sans-serif;
   

}

.cartTitle{
    color: black;
    font-family: "Dosis", sans-serif;
}

.total{
    color:black;
    font-family: "Dosis", sans-serif;
}

</style>