<template>
    <z-view style="border-width: 8px;"
    >

        <img class="mainclass" src="https://scontent-frt3-1.xx.fbcdn.net/v/t1.0-9/14708392_10207353879996909_3840106476384913590_n.jpg?_nc_cat=0&oh=8cd8c3aada72c3b7493dd8197c26c82d&oe=5C2A555E"
        >
        <div slot='extension'>

            <z-spot
                    button
                    slot='extension'
                    :angle='-50'
                    class='accent'
                    label='Github'
                    @click.native="openGithub">
                <i class='fab fa-github'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='10'
                    class='accent'
                    label='Facebook'
                    @click.native="openFacebook">
                <i class='fab fa-facebook'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='70'
                    class='accent'
                    label='Twitter'
                    @click.native="openTwitter">
                <i class='fab fa-twitter'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='130'
                    class='accent'
                    label='Linkedin'
                    @click.native="openLinkedin">
                <i class='fab fa-linkedin'></i>
            </z-spot>
            <z-spot
                    button
                    slot='extension'
                    :angle='180'
                    class='accent'
                    label='Mail'
                    @click.native="openMail">
                <i class='fa fa-safari'></i>
            </z-spot>
        </div>
    </z-view>



</template>
<script>
    export default {
        methods: {
            openGithub () {
                window.open('https://github.com/murat-aydin', '_blank')
            },
            openFacebook () {
                window.open('https://www.facebook.com/MurattAydnn', '_blank')
            },
            openTwitter () {
                window.open('https://twitter.com/Murataydin_61', '_blank')
            },
            openLinkedin () {
                window.open('https://www.linkedin.com/in/murataydin1/', '_blank')
            },
            openMail () {

            }

        }
    }
</script>
