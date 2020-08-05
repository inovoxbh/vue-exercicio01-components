<template>
    <div id="app">
        <img alt="Vue logo" src="./assets/logoPUC.png">
        <Header headerMsg="Exercício 01 - Vue - Componentização"/>
        <NavBar :menus="menus"/>
        <SideBar :menus="menus"/>
        <Articles :articles="articles"/>
    </div>
</template>

<script>
    import Header from './components/Header.vue';
    import NavBar from './components/NavBar.vue';
    import SideBar from './components/Side.vue';
    import Articles from './components/Articles.vue';

    export default {
        name: 'App',
        components: {
            Header,
            NavBar,
            SideBar,
            Articles
        },
        data() {
            return {
                menus: [
                    { id: 1, descricao: "menu01"},
                    { id: 2, descricao: "menu02"},
                    { id: 3, descricao: "menu03"},
                    { id: 4, descricao: "menu04"},
                    { id: 5, descricao: "menu05"}
                ],
                articles: [
                    { id: 1, descricao: "artigo01"},
                    { id: 2, descricao: "artigo02"},
                    { id: 3, descricao: "artigo03"},
                    { id: 4, descricao: "artigo04"},
                    { id: 5, descricao: "artigo05"}
                ]
            }
        }
    }
</script>

<style>
    #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    }

    h1 {
        color: darkgreen;
        font-weight: bold;
    }

    p {
        color: black;
    }

    ul{
        list-style-type:none;
    }

</style>
