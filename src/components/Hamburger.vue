<template>
    <button class="hamburger">
        <font-awesome-icon :icon="['fas', 'bars']" /> 
    </button>
    <div class="content-hamburger">
        <div class="header-content">
            <div class="welcome-text">
                Wellcome!
            </div>
            <div class="close-btn">
                <font-awesome-icon :icon="['fas', 'x']" />
            </div>
        </div>
        <div class="items-dropdown-btn">
            <div class="text-dropdown-btn">TV & Audio</div>
        </div>
    </div>
</template>

<script lang="ts">

export default {

}

</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
    
    .hamburger  {
        display: flex;
        width: 20px;
        height: 20px;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 8.333px;
        flex-shrink: 0;
        background-color: transparent;
        border: 0;
    }
    .close-btn {
        display: flex;
        width: 36px;
        height: 36px;
        justify-content: center;
        align-items: center;
        gap: 6px;
    }
    .content-hamburger {
        display: flex;
        background-color: transparent;
        width: 240px;
        padding-bottom: 0px;
        flex-direction: column;
        align-items: flex-start;
    }
    .welcome-text {
        color: #000;
        font-family: 'Roboto', sans-serif;
        font-size: 24px;
        font-weight: 500;
    }
    .header-content {
        display: flex;
        padding: 66px 20px 30px 20px;
        justify-content: space-between;
        align-items: center;
        align-self: stretch;
    }

    .items-dropdown-btn {
        display: flex;
        width: 240px;
        padding: 20px;
        justify-content: space-between;
        align-items: center;
    }
    .text-dropdown-btn {
        font-family: 'Roboto', sans-serif;
        font-size: 14px;
        font-style: normal;
        font-weight: 500;
        line-height: normal;
    }
</style>