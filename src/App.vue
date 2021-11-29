<template>
<div>

    <Appbar></Appbar>

    <v-container fluid>
      <router-view></router-view>
      </v-container>

      <v-footer app>
        </v-footer>
</div>
</template>
  
<script>
import Appbar from "@/components/Appbar"

export default {
  name: 'App',

  components: {
    Appbar,
  },

  data: () => ({
    //
  }),
};
</script>
