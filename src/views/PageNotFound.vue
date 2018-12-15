<template>
    <body>
        <div class="error">
            <div class="text-center">
                <h1>404 Error</h1>
                <h3 class="text-grey">Whoops! Looks like this page doesn't exist.</h3>
            </div>
        </div>
    </body>
</template>

<script>
    export default {
        name: "page-not-found"
    }
</script>

<style scoped>
    body {
        background-color: #f1f1f1;
        height: 40vh;
        border-bottom: 1px solid #e0e0e0;
    }

    h1 {
        font-family: 'Metropolis Black';
        color: #333;
    }

    h3 {
        font-family: 'Metropolis Thin'
    }

    .error {
        font-size: 150%;
    }

    .text-center {
        text-align: center;
        margin-top: 6%;
    }

    .text-grey {
        color: #9f9f9f;
    }
</style>