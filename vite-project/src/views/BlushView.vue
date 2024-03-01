<template>
    <div>
  <DestCard 
  v-for="blush in blush" 
  :key="blush.name"
  :Blush = "blush"
  />
    </div>
  </template>

<script setup>
import DestCard from "@/components/DestCard.vue";
const blush = 
[
        {
          name: "Soft Pinch Liquid Blush",
          brand: "Rare Beauty",
          color: "Grateful~ Bright Red",
          powder: false,
          price: "$23.00",
          img: "https://www.sephora.com/productimages/sku/s2362101-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Soft Pinch Liquid Blush",
          brand: "Rare Beauty",
          color: "Happy~ Cool Pink",
          powder: false,
          price: "$23.00",
          img: "https://www.sephora.com/productimages/sku/s2362085-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Soft Pinch Liquid Blush",
          brand: "Rare Beauty",
          color: "Encourage~ Neutral Pink",
          powder: false,
          price: "$23.00",
          img: "https://www.sephora.com/productimages/sku/s2518991-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Crème & Powder Blush Duo",
          brand: "Patrick Ta",
          color: "She's Vibrant!~ Bright Coral",
          powder: true,
          price: "$36.00",
          img: "https://www.sephora.com/productimages/sku/s2555894-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Crème & Powder Blush Duo",
          brand: "Patrick Ta",
          color: "She's Giving~ Cool Pink",
          powder: true,
          price: "$36.00",
          img: "https://www.sephora.com/productimages/sku/s2699353-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Crème & Powder Blush Duo",
          brand: "Patrick Ta",
          color: "She's A Doll~ Neutral Pink",
          powder: true,
          price: "$23.00",
          img: "https://www.sephora.com/productimages/sku/s2555886-main-zoom.jpg?imwidth=612",
        },
      ]

      </script>

<style scoped></style>