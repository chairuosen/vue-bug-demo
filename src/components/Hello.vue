<script>
    import Child from './Child.vue';
    import ToggleContent from './ToggleContent.vue';

    export default {
        name: 'hello',
        data () {
            return {
                msg: 'Welcome to Your Vue.js App',
            }
        },
        mounted: function () {

        },
        render(){
            var obj1 = {
                vnode:<ToggleContent title="works fine">
                    <div>works fine</div>
                </ToggleContent>
            };
            var obj2 = {
                vnode:<ToggleContent title="works not fine">
                    <a href="/">11111</a>
                </ToggleContent>
            }; // a2
            return <div>
                <Child obj={obj1}/>
                <Child obj={obj2}/>
            </div>
        }
    }
</script>
