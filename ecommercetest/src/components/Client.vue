<template>
    <v-row style="background-color: #080A21;">
               <v-col cols="3" sm="3" >
                 <v-card class="mx-auto my-12 pb-4" max-width="374" flat color="#080A21">
 
 
                   <v-card-item class="top-day">
                     <v-card-title class="text-center"
                       >Deals of the day</v-card-title
                     >
                   </v-card-item>
 
                   <v-card-text>
                     <div class="text-center">
                       <h1>Time Up</h1>
                     </div>
 
                   </v-card-text>
                 </v-card>
               </v-col>
               <v-col cols="3" sm="3" v-for="(client, i) in clients" :key="i">
                 <v-card class="mx-auto my-12 pb-4" max-width="374">
                   <v-img
                     height="250"
                     class="mx-4"
                     :src="client.img"
                   ></v-img>
 
                   <v-card-item class="mt-n4">
                     <v-card-title class="text-center"
                       >{{client.title}}</v-card-title
                     >
                   </v-card-item>
 
                   <v-card-text>
                     <div class="text-center">
                       {{client.bio}}
                     </div>
                     <v-row align="center" class="mx-0 mt-2">
                       <v-rating
                         :model-value="4.5"
                         color="amber"
                         density="compact"
                         half-increments
                         readonly
                         size="small"
                       ></v-rating>
                       <v-spacer></v-spacer>
                       <div class="text-grey ms-4">{{client.price}}</div>
                     </v-row>
                   </v-card-text>
                 </v-card>
               </v-col>
 
             </v-row>
 </template>
 
 <script>
 export default {
   data : ()=> ({
   clients: [
       {
         img: "Box1.png",
         title: "Box Counter 1",
         price: "$ 3",
         bio: " There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form,",
       },
       {
         img: "Box2.png",
         title: "Box Counter 2",
         price: "$ 9",
         bio: " There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form,",
       },
       {
         img: "Box3.png",
         title: "Box Counter 3",
         price: "$ 10",
         bio: " There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form,",
       },
 
     ]
 })
 }
 </script>
 
 <style>
 .top-day {
   margin-top: 120px;
 }
 </style>