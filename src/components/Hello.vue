<script>
    import Abc from './Abc.vue';

    export default {
        name: 'hello',
        data () {
            return {
                msg: 'Welcome to Your Vue.js App',
                idx:0,
            }
        },
        mounted: function () {

        },
        render(){

            var list = [
                <Abc title="this is component 0"></Abc>,
                <Abc title="this is component 1"></Abc>
            ];

            return <div>
                {list[this.idx]}
                <button onClick={ ()=> {
                    this.idx=0;
                }}>0</button>
                <button onClick={()=> {
                    this.idx=1;
                }}>1</button>
            </div>
        }
    }
</script>
