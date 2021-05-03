<template>
  <ion-app>
    <ion-router-outlet :animation="sampleAnimation" />
                  <!-- 👆👆👆👆👆👆👆👆👆👆👆👆👆👆👆 -->
                  <!-- this doesn't seem to work -->
  </ion-app>
</template>

<script lang="ts">
import { IonApp, IonRouterOutlet } from "@ionic/vue";
import { defineComponent } from "vue";
import sampleAnimation from "@/utils/Transition";

export default defineComponent({
  name: "App",
  components: {
    IonApp,
    IonRouterOutlet,
  },
  setup() {
    return { sampleAnimation };
  },
});
</script>