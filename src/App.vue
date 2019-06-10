<template>
    <div id="app" class="is-component">
        <router-view/>
    </div>
</template>

<script>
export default {
    name: "app"
};
</script>

<style type="text/scss" lang="scss">
@import "./styles/base";
html {
    height: 100%;
}
body {
    height: 100%;
	overflow: hidden;
}
#app {
    height: 100%;
}
#app.is-component {
    overflow: hidden;
}
</style>
