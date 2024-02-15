<template>
  <div>
<DestCard 
v-for="destination in destinations" 
:key="destination.name"
:Destination = "destination"
/>
  </div>
</template>

<script setup>
import DestCard from "@/components/DestCard.vue";
const destinations = 
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
        {
          name: "Better Than Sex Volumizing & Lengthening Mascara",
          brand: "Too Faced",
          color: "Black",
          price: "$29.00",
          img: "https://www.sephora.com/productimages/sku/s1533439-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Better Than Sex Volumizing & Lengthening Mascara",
          brand: "Too Faced",
          color: "Brown",
          price: "$29.00",
          img: "https://www.sephora.com/productimages/sku/s2600864-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Madeleine~ Light with Neutral Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s2172310-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Creme Brulee~ Light with Cool Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1847102-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Cannelle~ Light with Warm Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1847110-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Custard~ Medium with Neutral Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1478387-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Toffee~ Medium with Cool Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s2172344-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Macadamia~ Medium with Warm Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1847128-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Dark Coffee~ Deep with Neutral Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1847169-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Radiant Creamy Concealer",
          brand: "Nars",
          color: "Cacao~ Deep with Warm Undertones",
          price: "$32.00",
          img: "https://www.sephora.com/productimages/sku/s1478445-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "150~ Light with Neutral Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925171-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "170~ Light with Cool Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925197-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "180~ Light with Warm Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925205-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "260~ Medium with Neutral Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925288-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "200~ Medium with Cool Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925221-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "235~ Medium with Warm Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s2164630-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "450~ Deep with Neutral Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925478-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "480~ Deep with Cool Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925502-main-zoom.jpg?imwidth=612",
        },
        {
          name: "Pro Filt’r Soft Matte Liquid Foundation",
          brand: "Fenty Beauty",
          color: "440~ Deep with Warm Undertones",
          price: "$40.00",
          img: "https://www.sephora.com/productimages/sku/s1925460-main-zoom.jpg?imwidth=612",
        },









      ]
</script>

<style scoped></style>