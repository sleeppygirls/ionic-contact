<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Setting</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 3</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-list>

        <ion-list-header>Vue Basic Feature</ion-list-header>

        <ion-item @click="toState" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>State</h2>
            <p>State Management?</p>
          </ion-label>
        </ion-item>

        <ion-item @click="toIterator" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>Iterator - v-for</h2>
            <p></p>
          </ion-label>
        </ion-item>

        <ion-item @click="toIF" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>If Statement - v-if</h2>
            <p></p>
          </ion-label>
        </ion-item>

        <ion-item @click="toModal" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>Model - Two Data Binding - v-if</h2>
            <p></p>
          </ion-label>
        </ion-item>

        <ion-item @click="toEvent" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>Event</h2>
            <p></p>
          </ion-label>
        </ion-item>

        <ion-item @click="toLifecycle" class="ion-activatable ripple-parent">
          <ion-ripple-effect></ion-ripple-effect>
          <ion-label>
            <h2>Lifecycle</h2>
            <p></p>
          </ion-label>
        </ion-item>

      </ion-list>

    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { useRouter } from "vue-router";

const router = useRouter()

const toEvent = () => router.push({ path: '/vue/event' })
const toIF = () => router.push({ path: '/vue/if' })
const toIterator = () => router.push({ path: '/vue/iterator' })
const toLifecycle = () => router.push({ path: '/vue/lifecycle' })
const toModal = () => router.push({ path: '/vue/modal' })
const toState = () => router.push({ path: '/vue/state' })

</script>
