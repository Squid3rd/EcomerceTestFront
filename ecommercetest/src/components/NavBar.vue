<template>
    <v-app-bar flat>
        <template v-slot:prepend>
            <v-app-bar-nav-icon></v-app-bar-nav-icon>
        </template>

        <v-app-bar-title>Test Ecommerce with Vuelify</v-app-bar-title>
        
        <v-spacer></v-spacer>
        <v-text-field density="compact" variant="solo" label="Search products" append-inner-icon="mdi-magnify"
            single-line hide-details flat></v-text-field>

        <v-spacer></v-spacer>

        <v-btn> Sign In / Login </v-btn>
    </v-app-bar>
</template>

<script>
export default {};
</script>

<style></style>