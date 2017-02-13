<template>
  <div v-show="active">
1111
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
