<template>
    <Displayer :mystr="$route.params.word"/>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup() {

        const route = useRoute();
        const allowed_routes = ['/world', '/hello'];
        if (!allowed_routes.includes(route.path)) {
            navigateTo('/');
        }
    },
})
</script>

