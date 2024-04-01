<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-title>Todo Apps</ion-title>
            </ion-toolbar>
        </ion-header>
    </ion-page>
    <ion-content class="ion-padding">
        <ion-list>
            <ion-list-header>
                <ion-label>Data Kami</ion-label>
            </ion-list-header>
            <ion-item>
                <ion-label>
                    <h2>Putri</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum perspiciatis temporibus natus quaerat
                        cupiditate.</p>
                </ion-label>
            </ion-item>
            <ion-item>
                <ion-label>
                    <h2>Putri</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum perspiciatis temporibus natus quaerat
                        cupiditate.</p>
                </ion-label>
            </ion-item>
            <ion-item>
                <ion-label>
                    <h2>Putri</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum perspiciatis temporibus natus quaerat
                        cupiditate.</p>
                </ion-label>
            </ion-item>
            <ion-item>
                <ion-label>
                    <h2>Putri</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum perspiciatis temporibus natus quaerat
                        cupiditate.</p>
                </ion-label>
            </ion-item>
            <ion-item>
                <ion-label>
                    <h2>Putri</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum perspiciatis temporibus natus quaerat
                        cupiditate.</p>
                </ion-label>
            </ion-item>
        </ion-list>

        <ion-fab slot="fixed" horizontal="end" vertical="bottom">
            <ion-fab-button>
                <ion-icon :icon="add"></ion-icon>
            </ion-fab-button>
        </ion-fab>
    </ion-content>

    <ion-footer>
        <ion-toolbar>
            <ion-title>Putri &copy; 2024</ion-title>
        </ion-toolbar>
    </ion-footer>
</template>

<style>
ion-content {
    height: 83vh;
}

ion-fab-button {
    --background: #f399ce;
    --background-activated: #87d361;
    --background-hover: #a3e681;
    --border-radius: 15px;
    --box-shadow: 0px 1px 2px 0px rgba(0, 0, 0, 0.3), 0px 1px 3px 1px rgba(0, 0, 0, 0.15);
    --color: black;
}
</style>
<script lang="ts">
import { IonFab, IonFabButton, IonFabList, IonIcon } from '@ionic/vue';
import { add, colorPalette, document, globe } from 'ionicons/icons';
import { defineComponent } from 'vue';

export default defineComponent({
    components: { IonFab, IonFabButton, IonFabList, IonIcon },
    setup() {
        return { add };
    },
});
</script>

