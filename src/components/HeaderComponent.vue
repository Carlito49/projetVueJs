<template>
    <h1>Bienvenue sur le site de : {{ title }}</h1>
</template>

<script>

export default {
    name: "HeaderComponent",
    props: {
        title: String
    }
}

</script>

<style>

</style>



