<template>
<div class="container">


        <form>
        <fieldset>
            <legend>Music App</legend>
            
            <app-search></app-search>

        </fieldset>
        </form>

        <div class="col-md-12">
            Results  
        </div>


</div>

</template>

<script>

import SearchArea from './SearchArea.vue'

export default {
  components:{
    'app-search':SearchArea
    }
  }

</script>

<style></style>