<script>
    export default {
        props:{
            obj:true
        },
        data(){
            return {
                someObj:{}
            }
        },
        computed: {},
        methods: {},
        components: {},
        mounted(){
            this.someObj = this.obj; // a1
        },
        render(){
            return <div>
                {this.obj.vnode}
            </div>
        }
    }
</script>
