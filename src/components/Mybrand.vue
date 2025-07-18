<template>
    <div class="container">
    <img :src="icon" alt="Brand Icon" class="brand-icon" />
    <div class="mybrand">mysite</div>

    </div>
   
    

</template>

<script>
import icon from '../assets/icon.svg'
export default {
    name: 'Mybrand',
    data() {
        return {
            icon,
        };
    },
}

</script>

<style scoped>
.container {
    display: flex;
    align-items: center;
    gap: 1rem;
}
.brand-icon {
    width: 3rem;
    height: 3rem;
}

.mybrand {
    color: #fff;
    font-size: 1.5rem;
    
}

</style>