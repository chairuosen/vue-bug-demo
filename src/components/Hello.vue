<template>
  <div class="hello">
    <test1 class="item" ref="a"></test1>
    <test2 class="item" ref="b"></test2>
    <test3 class="item" ref="c"></test3>
  </div>
</template>

<script>
  import test1 from './test1.vue';
  import test2 from './test2.vue';
  import test3 from './test3.vue';

  export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
    test1,
    test2,
    test3
  },
  mounted:function () {
    this.$refs.a.show();
    this.$refs.b.show();
  }
}
</script>

<style scoped>
  .item{
    color:red;
  }
</style>
