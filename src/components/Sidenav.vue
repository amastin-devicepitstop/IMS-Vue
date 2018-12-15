<template>
    <div id="sidebar-container">
        <ul class="nav" id="sidebar">
            <tab-item title="Dashboard" icon="dashboard" :active="this.getRoute('Dashboard')"></tab-item>
            <navigation-divider></navigation-divider>
            <tab-item title="Store Stock" icon="storestock" :active="this.getRoute('Store Stock')"></tab-item>
            <tab-item title="Big Buys/Sales" icon="buysale" :active="this.getRoute('Big Buys/Sales')"></tab-item>
            <tab-item title="Returns" icon="returns" :active="this.getRoute('Returns')"></tab-item>
            <navigation-divider></navigation-divider>
            <tab-item title="Sign Maker" icon="signmaker" :active="this.getRoute('Sign Maker')"></tab-item>
            <tab-item title="Reports" icon="reports" :active="this.getRoute('Reports')"></tab-item>
        </ul>
    </div>

</template>

<script>
    import TabItem from '@/components/TabItem'
    import NavigationDivider from '@/components/NavigationDivider'
    export default {
        name: "sidenav",
        components: {
            TabItem,
            NavigationDivider
        },
        methods: {
            getRoute(val) {
                return this.$route.name === val;
            }
        }
    }
</script>

<style scoped>
    #sidebar-container {
        background: #2d373c;
        width: 12.5rem;
        border-right: 1px solid #e2e2e2;
        position: relative;
        z-index: 1;
    }

    #sidebar {
        padding-top: 12px;
        width: 12.5rem;
        height: -webkit-fill-available;
        bottom: -3.1rem;
        overflow-y: auto;
        position: fixed;
        background-color: inherit;
    }

    .nav {
        margin-bottom: 0;
        padding-left: 0;
        list-style: none;
    }


</style>