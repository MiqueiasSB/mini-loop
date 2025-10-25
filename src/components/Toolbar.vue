<script setup>
import { IonCol, IonGrid, IonRow } from '@ionic/vue';

</script>

<template>
    <ion-header>
        <ion-toolbar>
            <ion-grid>
                <ion-row class="ion-align-items-center">
                    <ion-col size="auto">
                        <ion-img id="logo" src="resources/logo.svg" alt="logo"></ion-img>
                    </ion-col>
                    <ion-col>
                        <ion-title class="logo-font">Mini Loop</ion-title>
                    </ion-col>

                </ion-row>
            </ion-grid>

        </ion-toolbar>
    </ion-header>
</template>

<style lang="scss">
ion-header {
    margin-bottom: 2em;

    #logo {
        width: 2.5em;
    }

    ion-title {
        padding-left: 0%;
        font-size: 2em;
    }
}
</style>