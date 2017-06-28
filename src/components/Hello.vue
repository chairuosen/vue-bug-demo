<script>
    import Child from './Child.vue';
    import ToggleContent from './ToggleContent.vue';
    import Abc from './Abc.vue';

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
                vnode:<ToggleContent title="this works not fine. click me">
                    <a href="/">11111</a>
                </ToggleContent>
            }; // a2
            var obj3 = {
                vnode:<Abc>
                    <a href="/">But this component works also fine with `a` tag.</a>
                </Abc>
            };
            return <div>
                <Child obj={obj1}/>
                <Child obj={obj2}/>
                <Child obj={obj3}/>
            </div>
        }
    }
</script>
