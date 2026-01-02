<template>
    <div v-html=svg class="svg">
    </div>
</template>

<script setup>

    const props = defineProps(['fill', 'stroke', 'src'])
    const fill = props.fill || 'none'
    const stroke = props.stroke || 'none'

    const svgUrl = await $fetch("http://localhost:3000"+props.src)
    const svgText = await svgUrl.text()
    let svg = svgText.replace(/\sfill\=\"([^\"]+)\"/gm, `fill="${fill}"`)
    svg = svg.replace(/\sstroke\=\"([^\"]+)\"/gm, `stroke="${stroke}"`)
    svg = svg.replace(/\swidth\=\"([^\"]+)\"/gm, ``)
    svg = svg.replace(/\sheight\=\"([^\"]+)\"/gm, ``)
</script>

<style>

    .svg {
        width: 100%;
        position: absolute;
        top: 0;
        left: 0;
    }
</style>