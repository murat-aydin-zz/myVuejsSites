<template>
    <z-view>
        <section slot="extension">
            <z-list
                    :items="devices"
                    :per-page="10">
                <z-spot
                        slot-scope="props"
                        :index="props.index"

                        :label="props.category">
                    <span style="color: white;">{{props.qty}}</span>
                    <z-spot slot="extension"
                            :style="props.category === 'care' ? 'background-color: red; border: none;': 'background-color: green; border: none;'"
                            :angle='-45'
                            size='xxs'>
                    </z-spot>
                </z-spot>
            </z-list>
        </section>
    </z-view>
</template>
<script>
    export default {
        data () {
            return {
                devices: [
                    {category: 'JAVA', qty: '7/10'},
                    {category: 'C#',  qty: '6/10'},
                    {category: 'Android Geliştirme',  qty: '7/10'},
                    {category: 'Php / Laravel',  qty: '7/10'},
                    {category: 'Vue.js',  qty: '7/10'},
                    {category: 'Javascript',  qty: '6/10'},
                    {category: 'Html/ Css',  qty: '8/10'},
                    {category: 'Unity',  qty: '6/10'},
                    {category: 'React.js',  qty: '3/10'},

                ]
            }
        }
    }
</script>