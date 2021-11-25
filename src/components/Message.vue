<template>
    <div class="shadow p-3 mb-5 bg-body border rounded" :class="`border-${mensaje.tipo}`">
        <h4 class="text-center text-uppercase">{{ mensaje.usuario }}</h4>
        <p class="text-center">
            {{ mensaje.msg }}
        </p>
    </div>
</template>

<script>
    export default {
        props: {
            mensaje: {
                type: Object,
                default: () => {}
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>