<template>
    <z-view style="border-width: 8px;"
    >

        <img class="mainclass" src="https://scontent-frt3-1.xx.fbcdn.net/v/t1.0-9/14708392_10207353879996909_3840106476384913590_n.jpg?_nc_cat=0&oh=8cd8c3aada72c3b7493dd8197c26c82d&oe=5C2A555E"
        >
        <div slot='extension'>

            <z-spot
                    button
                    slot='extension'
                    :angle='135'
                    class='accent'
                    label='Github'
                    @click.native="openGithub">
                <i class='fab fa-github'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='135'
                    class='accent'
                    label='Facebook'
                    @click.native="openFacebook">
                <i class='fab fa-github'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='135'
                    class='accent'
                    label='Twitter'
                    @click.native="openTwitter">
                <i class='fab fa-github'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='135'
                    class='accent'
                    label='Linkedin'
                    @click.native="openLinkedin">
                <i class='fab fa-github'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='135'
                    class='accent'
                    label='Mail'
                    @click.native="openMail">
                <i class="fab fa-google"></i>
            </z-spot>
        </div>
    </z-view>



</template>
<script>
    export default {
        methods: {
            openGithub () {
                window.open('https://github.com/zircleUI/zircleUI', '_blank')
            },
            openFacebook () {
                window.open('https://github.com/zircleUI/zircleUI', '_blank')
            },
            openTwitter () {
                window.open('https://github.com/zircleUI/zircleUI', '_blank')
            },
            openLinkedin () {
                window.open('https://github.com/zircleUI/zircleUI', '_blank')
            },
            openMail () {
                window.open('https://github.com/zircleUI/zircleUI', '_blank')
            }

        }
    }
</script>
