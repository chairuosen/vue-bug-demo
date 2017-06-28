<style lang="less" type="text/less" scoped>

</style>
<template>
    <div>
        {{title}}
        {{count}}
        <button @click="count++">+</button>
    </div>
</template>
<script type="text/ecmascript-6">
    export default {
        props:['title'],
        data(){
            return {
                count:0
            }
        },
        computed: {},
        methods: {},
        components: {},
        mounted(){

        }
    }
</script>
