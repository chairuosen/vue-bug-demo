<template>
  <div v-if="active">
      3333
  </div>
</template>

<script>
  export default {
    data () {
      return {
        active:true
      }
    },
    methods:{
      show:function () {
        this.active = true;
      }
    }
  }
</script>
