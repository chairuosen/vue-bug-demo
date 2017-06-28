<style lang="less" type="text/less" scoped>
    .title{
        position:relative;
        background:#eee;
        color:#333;
        font-weight:bold;
        font-size:16px;
        padding:0 10px;
        line-height:2em;
        &:after{
            content:'v';
            font-weight:normal;
            display:block;
            position:absolute;
            right:10px;
            top:0;
        }
        &.show{
            &:after{
                transform: rotateX(180deg);
            }
        }
    }
    .body{
        margin-bottom:10px;
    }
    ._content{
        padding:10px;
    }
</style>
<template>
    <div class="body">
        <div class="title" :class="{show:show}" @click="show = !show">
            {{title}}
        </div>
        <div class="_content" v-show="show">
            <slot></slot>
        </div>
    </div>
</template>
<script type="text/ecmascript-6">
    export default {
        props:{
            title:String
        },
        data(){
            return {
                show:false
            }
        },
        computed: {},
        methods: {},
        components: {},
        mounted(){
        }
    }
</script>
