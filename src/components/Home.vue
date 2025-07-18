<template>
    <nav class="nav">
        <!-- Mybrand component is imported and used here -->
        <Mybrand />
        
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
    padding: 0.3rem;
    background-color: #1a382a;
    

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
    all: unset;
    margin-left: 0.5rem;
    gap: 1rem;
    height: 1rem;
    padding: 0.5rem 1rem;
    text-align: center;
    border-radius: 0.5rem;
    background-color: #1a382a;
    color: #fff;
    transition: 0.3s ease-in-out all;
 
}
.btn:hover{
    background-color: #fff;
    color: #1a382a;
    cursor: pointer;
    transform: scale(1.05);
}




</style>