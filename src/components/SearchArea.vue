<template>

      <div class="form-group ">
            <label for="inputEmail" class="col-lg-2 control-label">Search Music</label>
            <div class="col-lg-10">
                <input type="text" class="form-control" id="inputEmail" placeholder="Type here.." @input="keyPressed">
            </div>
      </div>

</template>

<script>

export default{
 
    methods:{

            keyPressed(event){
                var key = event.target.value;
            
                cosole.log(key)
            }



    }


}

</script>

<style></style>