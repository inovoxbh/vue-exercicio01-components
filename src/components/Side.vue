<template>
    <div>
        <h1>SideBar</h1>
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
        name: 'Side',
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
    div {
        background-color: lightgreen;
    }
</style>
