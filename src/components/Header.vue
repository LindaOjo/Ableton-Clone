<template>
    <div class="header flex-row">
        <div class="flex-row"> 
        <Logo/>
        <ul class="flex-row">
            <li>Live</li>
            <li>Push</li>
            <li>Link</li>
            <li>Shop</li>
            <li>Packs</li>
            <li>Help</li>
            <li>More +</li>
        </ul>
       </div>

        <ul class="flex-row">
           <li class="blue-text">Try Live for free</li>
           <li class="small-links">Log in or register</li>
       </ul>
    </div>
</template>

<script>

import Logo from "./Logo.vue";


    export default {
        name: 'Header',
        components: {
            Logo
        }
        
    }
</script>

<style scoped lang="scss">
.header {
    display: flex;
    justify-content: space-between;
    padding: 1.25rem 0;
    margin: 0 2.5rem;
    height: auto;
    width: auto;
    font-size: 20px;
}

ul {
   align-items: center;
}

li {
    margin: 0 1.5rem;
}

.blue-text {
    color: #0000ff;
}

.small-links {
    font-size: 16px;
}

</style>