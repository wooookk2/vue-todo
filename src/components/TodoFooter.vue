<template>
  <div class="clearAllContainer">
      <span class="claerAllBtn" v-on:click="clearTodo">Clear All</span>
  </div>
</template>

<script>
export default {
    methods : {
        clearTodo : function(){
            this.$emit('clearAll')
        }
    }
}
</script>

<style scoped>
.clearAllContainer{
    width: 8.5rem;
    height: 50px;
    line-height: 50px;
    background-color: white;
    border-radius: 5px;
    margin: 0 auto
}
.claerAllBtn{
    color: #e20303;
    display: block;;
}
</style>