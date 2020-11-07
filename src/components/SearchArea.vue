<template>

      <div class="form-group ">
            <label for="inputEmail" class="col-lg-2 control-label">Search Music</label>
            <div class="col-lg-10">
                <input type="text" class="form-control" id="inputEmail" placeholder="Type here" @input="keyPressed">
            </div>
      </div>

</template>

<script>

import axios from 'axios'

export default{
 
    methods:{

            keyPressed(event){
              var key = event.target.value;
            
            axios.get("https://api.spotify.com/v1/search?q="+ key + "&type=tracks")
                 .then(response=>{
                     console.log(response.data)
                 })
                 .catch(e=>{
                     this.error.push(e)
                 })

            }



    }


}

</script>
