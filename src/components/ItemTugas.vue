<template>
    <div class="div">
         <input class="form-check-input" 
              type="checkbox" 
              id="defaultCheck1">
              <label 
              class="form-check-label item" 
              v-bind:class="{'item-complate':tugasSaya.isDone}" 
              for="defaultCheck1">{{ tugasSaya.nama }}</label>
    </div>
</template>

<script>
export default {
    
}
</script>
<style scoped>

</style>