<template>
    <div>{{link.description}} ({{link.url}})</div>
</template>

<script>
    export default {
        name: 'testgraphql',
        props: ['link']
    }
</script>