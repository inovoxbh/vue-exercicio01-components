<template>
    <div>
        <h1>Articles</h1>
        <ul>
            <li v-for="articleArray in articles" v-bind:key="articleArray.id">
                <ArticleItem :article="articleArray"/>
            </li>
        </ul>
    </div>
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
    h1 {
        color: darkgreen;
    }
    ul{
        list-style-type:none;
    }
    li {
        color:red;
    }
</style>
