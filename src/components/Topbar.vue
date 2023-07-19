<template>
    <div class="topbar-container">
            <DropdownBtn />
        <div class="right-container">
            <div class="social-container">
                <a class="social-links" href="#"> <font-awesome-icon :icon="['fab', 'facebook-f']" /> </a>
                <a class="social-links" href="#"> <font-awesome-icon :icon="['fab', 'instagram']" /> </a>
                <a class="social-links" href="#"> <font-awesome-icon :icon="['fab', 'linkedin-in']" /> </a>
                <a class="social-links" href="#"> <font-awesome-icon :icon="['fab', 'twitter']" /> </a>
                <a class="social-links" href="#"> <font-awesome-icon :icon="['fab', 'youtube']" /> </a>
            </div>
            <div class="services-container">
                <a class="services-links" href=""> <font-awesome-icon :icon="['fas', 'location-dot']" /> Track Order</a>
                <a class="services-links" href=""> <font-awesome-icon :icon="['fas', 'store']" /> Shop</a>
                <a class="services-links" href=""> <font-awesome-icon :icon="['fas', 'gear']" /> Settings</a>
                <a class="services-links" href=""> FAQ </a>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import DropdownBtn from '@/components/DropdownBtn.vue';

export default {
    components: {
        DropdownBtn,
    }
}
</script>

<style scoped>
    .topbar-container {
        display: flex;
        padding: 8px 240px;
        justify-content: space-between;
        align-items: center;
        align-self: stretch;
    }
    .services-container {
        display: flex;
        padding: 2px 24px;
        justify-content: center;
        align-items: center;
        gap: 24px;
    }
    .social-container {
        display: flex;
        padding-right: 0px;
        justify-content: center;
        align-items: center;
        gap: 20px;
    }
    .right-container {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .social-links {
        color: grey;
        text-decoration: none;
    }
    .services-links {
        color: grey;
        text-decoration: none;
        padding: 2px 24px;
        border-left: 1px solid var(--grey-100, grey);
    }
</style>