<template>
<div class="container">


        <form>
        <fieldset>
            <legend>Music App</legend>
            
            <app-search></app-search>

        </fieldset>
        </form>

        <div class="col-md-12">
            <app-result></app-result>
        </div>


</div>

</template>

<script>

import SearchArea from './SearchArea.vue'
import ResultArea from './ResultArea.vue'

export default {
  components:{

    'app-search':SearchArea,
    'app-result':ResultArea,

    }
  }

</script>

<style></style>