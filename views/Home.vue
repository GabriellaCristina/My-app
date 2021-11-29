<template>
  <div>
    <v-row >
      <v-col
        v-for="{data,i} in myCards"
        :key="i"
        cols="12"
        sm="6"
        md="4"
        xs="2"
        
      >
      {{data}}
      <Mycard> :cardid= "i" :cardInfo="data"> </Mycard>
      
        
      </v-col>
    </v-row>
    
  </div>
</template>

<script>
import Mycard from '../components/Mycard'


export default {
    name: 'Home',
    data(){
      return {
        titleview: this.Sstore.state.title
      }
    },

    components: {
        Mycard(){
          return this.$store.state.cards
        },
       
    },
    components: {
        Mycard,
}
}
</script>
