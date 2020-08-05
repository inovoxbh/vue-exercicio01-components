<template>
    <div>
        <h1>NavBar</h1>
        <ul>
            <li v-for="menuArray in menus" v-bind:key="menuArray.id">
                <NavItem :menu="menuArray"/>
            </li>
        </ul>
    </div>
</template>

<script>
    import NavItem from './NavItem';

    export default {
        name: 'NavBar',
        components: {
            NavItem
        },
        props: {
            menus: Array
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
