<template>
    <z-view>
        <section slot="extension">
            <z-list
                    :items="devices"
                    :per-page="1">
                <z-spot
                        slot-scope="props"
                        :index="props.index"
                        :to-view="{ name: 'device', params: { fruit: props.category}}"
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
                    {category: 'Fırat Üniversitesi - Yazılım Mühendisliği', qty: 2.80+'/4 Ort'},
                    {category: 'Dobo Creative Agency - Software Developer', qty: 4+'ay'},
                    {category: 'Kokteyl Bil. Hiz- Android Developer', qty: 5+'ay'},
                    {category: 'Dotto Bil. Tek- Game Developer', qty: 4+'ay'},
                    {category: 'Weecomi - Mobil & Web Developer', qty: 5+'ay'},
                    {category: 'Ubit - Web Developer', qty: 5+'ay'},
                    {category: 'Toplam Tecrübe', qty: 2+'yıl'},


                ]
            }
        }
    }
</script>