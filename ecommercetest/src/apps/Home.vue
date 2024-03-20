<template>
    <v-app>
        <NavBar />
        <v-main>
            <v-container>
                <v-row>
                    <v-col>

                        <v-carousel>
                            <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src">
                                <v-row>
                                    <v-col cols="12" sm="6">
                                        <div class="d-flex fill-height justify-center align-center">
                                            <h2 class="text-white-top">
                                                {{ item.title }}
                                            </h2>
                                        </div>
                                        <div class="d-flex fill-height justify-center align-center">
                                            <h2 class="text-white-top">
                                                {{ item.text }}
                                            </h2>
                                        </div>
                                        <div class="d-flex fill-height justify-center align-center">
                                            <v-btn color="success">Buy Now</v-btn>
                                        </div>
                                    </v-col>

                                </v-row>
                            </v-carousel-item>
                        </v-carousel>
                    </v-col>
                    <v-toolbar color="transparent">
                        <v-toolbar-title>Popular Products</v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-btn icon="mdi mdi-chevron-left"></v-btn>
                        <v-btn icon="mdi mdi-chevron-right"></v-btn>
                    </v-toolbar>
                    <v-col cols="12" sm="12" class="mt-n10">
                        <Populars />
                    </v-col>
                    <v-toolbar color="transparent" class="mt-n10">
                        <v-toolbar-title>Featured Products</v-toolbar-title>
                        <v-spacer></v-spacer>
                        <v-btn icon="mdi mdi-chevron-left"></v-btn>
                        <v-btn icon="mdi mdi-chevron-right"></v-btn>
                    </v-toolbar>
                    <v-col cols="12" sm="12" class="mt-n10">
                        <Features />
                    </v-col>
                    <v-col cols="12" sm="12" class="mt-n10">
                        <Client />
                    </v-col>

                </v-row>
            </v-container>
        </v-main>
    </v-app>
</template>

<!-- <script setup>

</script> -->

<script>
export default {
    data() {
        return {
            items: [
                {
                    src: "Box1.png",
                    title: "Box Counter 1",
                    text: "Another Description"
                },
                {
                    src: "Box2.png",
                    title: "Box Counter 2",
                    text: "Another Description"
                },
                {
                    src: "Box3.png",
                    title: "Box Counter 3",
                    text: "Another Description"
                },
                {
                    src: "Box4.png",
                    title: "Box Counter 4",
                    text: "Another Description"
                },
                {
                    src: "Box5.png",
                    title: "Box Counter 5",
                    text: "Another Description"
                },
                {
                    src: "Box6.png",
                    title: "Box Counter 6",
                    text: "Another Description"
                },
                {
                    src: "Box1.png",
                    title: "Box Counter 1",
                    text: "Another Description"
                },
            ]
        }
    },
}
</script>

<style scoped>
.top {
  margin-top: 100px;
}
.text {
  margin-top: -40px;
  margin-left: 80px;
}
.top-day {
  margin-top: 120px;
}
</style>