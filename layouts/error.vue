<template>
    <div>
        <h1 v-if="error.statusCode === 404">Pagina Non trovata</h1>
        <h1 v-else>Ops... Un errore... :(</h1>
        <NuxtLink to="/">Ritorna alla Home Page</NuxtLink>
        <Nuxt />
    </div>
</template>

<script>
export default {
    props: ['error'],
    layout: 'error'
}
</script>

<style>

</style>