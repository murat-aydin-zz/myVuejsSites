<template>
    <z-view label="Home status" style="background-color: black">
        <canvas slot="media" id="smoothie-chart" style="height:50%; width: inherit;"></canvas>
        <div slot="extension">
            <z-spot
                    :angle="-45"
                    size="m"
                    :distance="120"
                    label="Events"
                    @click.native="iletisim">
                15
            </z-spot>
        </div>
    </z-view>
</template>
<script>

</script>