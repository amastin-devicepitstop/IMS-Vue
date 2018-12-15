<template>
  <div id="app">
    <navigation v-if="this.pageKnown()"></navigation>
    <router-view/>
  </div>
</template>

<script>
    import Navigation from '@/components/Navigation'
    export default {
        name: 'App',
        components: {
            Navigation
        },
        data() {
            return {

            }
        },
        methods: {
            pageKnown() {
                return this.$route.name !== "Page Not Found"
            }
        }
    }
</script>

<style>
    @font-face {
        font-family: 'Metropolis Thin';
        src: url(./assets/fonts/Metropolis-Thin.ttf)
    }

    @font-face {
        font-family: 'Metropolis Light';
        src: url(./assets/fonts/Metropolis-Light.ttf)
    }

    @font-face {
        font-family: 'Metropolis Regular';
        src: url(./assets/fonts/Metropolis-Regular.ttf)

    }

    @font-face {
        font-family: 'Metropolis Medium';
        src: url(./assets/fonts/Metropolis-Medium.ttf)
    }

    @font-face {
        font-family: 'Metropolis SemiBold';
        src: url(./assets/fonts/Metropolis-SemiBold.ttf)
    }

    @font-face {
        font-family: 'Metropolis Bold';
        src: url(./assets/fonts/Metropolis-Bold.ttf)
    }

    @font-face {
        font-family: 'Metropolis Black';
        src: url(./assets/fonts/Metropolis-Black.ttf)
    }

    html, body {
        height: 100%;
        width: 100%;
        margin: 0;
        padding: 0;
        overflow-x: hidden;
    }

    body {
        line-height: 1.42857143;
        color: #222;
        font-family: 'Metropolis Regular', 'Helvetica', 'Arial', sans-serif;
        font-size: 15px;
        letter-spacing: -0.045rem;
    }

    *:focus {
        outline: 0;
    }
/*#app {*/
  /*font-family: 'Metropolis Regular';*/
/*}*/
/*#nav {*/
  /*padding: 30px;*/
/*}*/

/*#nav a {*/
  /*font-weight: bold;*/
  /*color: #2c3e50;*/
/*}*/

/*#nav a.router-link-exact-active {*/
  /*color: #42b983;*/
/*}*/
</style>
