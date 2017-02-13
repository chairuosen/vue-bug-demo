<template>
  <div v-if="active">
      2222
  </div>
</template>

<script>
  export default {
    data () {
      return {
        active:false
      }
    },
    methods:{
      show:function () {
        this.active = true;
      }
    }
  }
</script>
