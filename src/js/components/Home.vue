<template>
  <div>
   <h3>TOP SECTION</h3>
   <p>There are <i>{{count}}</i> Post.</p>
    
   <input placeholder="paste your token" type="text" @change="updateApi">
  </div>
</template>
<script>
import { mapState, mapMutations, mapActions, mapGetters } from 'vuex'
export default {
  components: {
    
  },
  data: function() {
    return {
      
    };
  },
  props: {
   
  },
  beforeMount() {
  },
  computed: {
    count () {
        return this.$store.state.posts.count
      },
  },
  mounted() {
    
  },

  beforeDestroy() {},

  methods: {
   ...mapActions('posts/',[
    'updateApi',
   ]),
    
    
  }
};
</script>

<style scoped>

</style>