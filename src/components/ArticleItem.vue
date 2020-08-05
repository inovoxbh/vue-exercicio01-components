<template>
    <p>{{ article.descricao }}</p>
</template>

<script>
    export default {
        name: 'ArticleItem',
        props: {
            article: Object
        }
    };
</script>
