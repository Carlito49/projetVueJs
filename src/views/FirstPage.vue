<template>
    <div>
        <HeaderComponent title="Moi"/>
    </div>
    <div>
        <FormComponent />
    </div>
</template>

<script>

import FormComponent from '../components/FormComponent.vue';
import HeaderComponent from '../components/HeaderComponent.vue';

export default {
    components: {
        FormComponent,
        HeaderComponent
    }
}

</script>

<style>

</style>