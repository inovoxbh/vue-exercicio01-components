<template>
    <p>{{ menu.descricao }}</p>
</template>

<script>
    export default {
        name: 'NavItem',
        props: {
            menu: Object
        }
    };
</script>
