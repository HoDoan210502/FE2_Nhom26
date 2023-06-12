<template>
    <v-app-bar app color="black" dark flat class="px-12 navbar">
        <v-btn>
            <v-icon color="white" class="mr-2"><i class="fa-solid fa-signature">Electro</i></v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-col cols="6">
        <v-text-field density="compact" variant="outlined" label="Search" single-line hide-details class="mr-2"></v-text-field>
    </v-col>
        <v-btn text @click="scroll('home')" class="text-yellow">Home</v-btn>
        <v-btn text @click="scroll('service')">Service</v-btn>
        <v-btn text @click="scroll('page')">Page</v-btn>
        <v-btn text @click="scroll('about')">About</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
        <v-btn>Account</v-btn>
    </v-app-bar>
</template>
<script>
    export default{
        methods:{
            scroll(refName){
                const element = document.getElementById(refName);
                element.scrollIntoView({behavior:"smooth"});
            }
        }
    }
</script>
<style>
</style>