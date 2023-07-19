<template>
  <Topbar />
  <Navbar />
</template>

<script lang="ts">
import Topbar from '@/components/Topbar.vue';
import Navbar from '@/components/Navbar.vue';


import { library } from '@fortawesome/fontawesome-svg-core'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faUserSecret } from '@fortawesome/free-solid-svg-icons'


export default {
  components: {
    Topbar,
    Navbar,
    
  },
}


</script>
