<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-buttons slot="start">
                    <ion-button @click="back">
                        <ion-icon slot="icon-only" :icon="arrowBackOutline"></ion-icon>
                    </ion-button>
                </ion-buttons>
                <ion-title>IF</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content :fullscreen="true">

            <ion-header collapse="condense">
                <ion-toolbar>
                    <ion-title size="large">IF</ion-title>
                </ion-toolbar>
            </ion-header>

            <div v-if="jk == 1">
                <h2>Laki-Laki</h2>
            </div>

            <div v-else>
                <h2>Perempuan</h2>
            </div>

            <ion-button @click="rubahKelamin" expand="block" fill="solid">Click Me</ion-button>

            <div v-if="jk == 1">
                <h2>Laki-Laki</h2>
            </div>

            <div v-else>
                <h2>Perempuan</h2>
            </div>

            <ion-button @click="rubahKelamin" expand="block" fill="solid">Click Me</ion-button>
        
        </ion-content>
    </ion-page>
</template>

<script setup>
import { ref } from "vue";
import { useRouter } from 'vue-router';
import { arrowBackOutline } from 'ionicons/icons';

const router = useRouter()

const back = () => {
    router.back()
}

// variabel biasa
let jk = 2 // 1: Laki-Laki | 2: Perempuan
let gender = ref(2) // 1: Laki-Laki | 2: Perempuan

// function rubah kelamin
const rubahKelamin = () => {
    // if biasa
    if(jk ==1) {
        jk = 2
    } else {
        jk = 1
    }

    // tertiary
    jk = jk == 1 ? 2 : 1
}

const rubahGender = () => {
    gender.value = gender.value == 1 ? 2 : 1
}
</script>

<style></style>