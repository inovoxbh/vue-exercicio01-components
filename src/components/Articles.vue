<template>
    <article>
        <h1>Articles</h1>
        <ul>
            <li v-for="articleArray in articles" v-bind:key="articleArray.id">
                <ArticleItem :article="articleArray"/>
            </li>
        </ul>
    </article>
</template>

<script>
    import ArticleItem from './ArticleItem';

    export default {
        name: 'Articles',
        components: {
            ArticleItem
        },
        props: {
            articles: Array
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    article {
        background-color: gray;
    }
</style>
