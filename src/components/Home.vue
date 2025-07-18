<template>
    <nav class="nav">
        <Mybrand />
        <!-- Mybrand component is imported and used here -->
         <!-- Navigation links -->
        <ul class="navlink"> 
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
        <div class="resgistration">
            <button class="btn">Login</button>
            <button class="btn">Sign Up</button>
        </div>
    </nav>
</template>

<script>
import Mybrand from './Mybrand.vue'
export default{
    name: 'Navbars',
    components: {
        Mybrand
    }
}
</script>

<style scoped>
.nav{
    display: flex;
    justify-content: space-between; /* pushes first and last items to ends */
    align-items: center;
    flex-wrap: nowrap;
    padding: 1.2rem;
    background-color: #333;
    

}

.navlink{
    display: flex;
    list-style: none;
    gap: 1.2rem;
    padding-left: 3rem;
   
}
.navlink li a{
    text-decoration: none;
    color: #fff;
    font-size: 1.2rem;
   
}
.registration{
    display: flex;
    gap: 1.2rem;
    justify-content: space-between;
    align-items: center;
   
}
.btn{
    margin-left: 0.7rem;
}




</style>