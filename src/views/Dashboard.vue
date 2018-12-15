<template>
  <div class="dashboard">

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Navbar from '@/components/Navigation.vue'; // @ is an alias to /src

@Component({
  components: {
    Navbar,
  },
})
export default class Dashboard extends Vue {}
</script>
