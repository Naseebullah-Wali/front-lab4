// <template> 
  <Header v-bind="headerParams"/>
  <router-view />
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
  },
  data() {
    return {
      headerParams: {
        variant: "3287",
        group: "P3232",
        firstName: "Naseebullah",
        lastName: "Wali"
      }
    }
  }
}
</script>

<style>
@import url('http://fonts.googleapis.com/css?family=Roboto');

body{
    /* background-color: #564F6F; */
    background-color: whitesmoke;
    /* color: whitesmoke; */
    
    /*margin-left: 20px;*/
    /*margin-right: 30px;*/
    /*width: auto;*/

}

#app {
  font-family: Roboto, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* color: #2c3e50; */
}

</style>
