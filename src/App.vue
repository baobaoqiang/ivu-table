<template>
    <div id="app">
        <div id="nav">
            <router-link to="/">Home</router-link> |
            <router-link to="/about" replace>Table</router-link>
        </div>
        <router-view />
    </div>
</template>

<style lang="scss">
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    padding: 0 80px;
}

#nav {
    padding: 30px;

    a {
        font-weight: bold;
        color: #2c3e50;
        display: inline-block;

        &.router-link-exact-active {
            color: #42b983;
            border-bottom: 1px solid #42b983;
        }
    }
}
</style>
