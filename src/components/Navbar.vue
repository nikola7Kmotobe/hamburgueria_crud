<template>
    <div>
        <nav id="nav">
            <router-link id="logo-url" to="/">
                <img :src="img_src" :alt="alt" id="logo">
            </router-link>
            
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/pedidos">Pedidos</RouterLink>
            
        </nav>
    </div> 
</template>

<script>
    export default{
        name:"Navbar",
        props:{
            img_src: String,
            alt: String
        }
    }
</script>

<style scoped>
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }

  #nav #logo-url {
    margin: auto;
    margin-left: 0;
  }

  #logo {
    width: 40px;
    height: 40px;
  }

  #nav a {
    color: #fcba03;
    text-decoration: none;
    margin: 12px;
    transition: .5s;
  }

  #nav a:hover {
    color: #FFF;
  }
</style>