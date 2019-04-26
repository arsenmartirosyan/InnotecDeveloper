<template>
    <div id="main">
        <header id="header">
            <h1>
                <router-link :to="{name: 'home'}">
                   Home
                </router-link>
            </h1>
            <navigationMenu></navigationMenu>
        </header>
        <div id="content">
            <router-view></router-view>
        </div>
    </div>
</template>
<script>
    import navigationMenu from './components/Menu.vue'
    export default {
        data() {
            return {
                //
            }
        },
        components: {
            navigationMenu
        }
    }
</script>