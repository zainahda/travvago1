<template>
  <div>
  <b-navbar toggleable="lg" type="light">
        <div class="container navbar">
            <b-img src="../assets/logo.png" width="50px"></b-img>
            <b-navbar-brand class="nav-brand" href="#">TravvaGo</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav class="navbar-link ml-auto">
                <router-link class="nav-link" to="/">Home |</router-link>
                <router-link class="nav-link" to="/destinations">Destinations |</router-link>
                <router-link class="nav-link" to="/">Galery |</router-link>
            </b-navbar-nav>
                <b-button class="btn btn-login" href="../users/login"><svg width="20px" height="20px" viewBox="0 0 16 16" class="bi bi-person-circle" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                    <path d="M13.468 12.37C12.758 11.226 11.195 10 8 10s-4.757 1.225-5.468 2.37A6.987 6.987 0 0 0 8 15a6.987 6.987 0 0 0 5.468-2.63z"/>
                    <path fill-rule="evenodd" d="M8 9a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"/>
                    <path fill-rule="evenodd" d="M8 1a7 7 0 1 0 0 14A7 7 0 0 0 8 1zM0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8z"/>
                    </svg> Login </b-button>
                    <b-button class="btn btn-signup" href="#">Sign up</b-button>
                    
            </b-collapse>
        </div>
    </b-navbar>
    </div>
</template>

<script>
  export default {
    name: 'Navbar',
  }
</script>

<style scoped>
.navbar {
    position: relative;
    z-index: 1;
}
.navbar-brand {
    font-family: 'Irish Grover', cursive;
    font-size: 26px;
}
.navbar-nav {
    text-transform: uppercase;
    margin-right: 20px;
}
.navbar-brand, .nav-link, .btn-login{
    color: #F85E1D !important;
    text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.41);
}
.btn-login{
    margin-left: 0px;
    background: none;
    border: none;

}
.btn-signup {
    background: linear-gradient(180deg, #FEA858 0%, #F85E1D 100%);
    box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.btn:active {
    position: relative;
    top: 7px;
    box-shadow: none;
}

/* tablet version */
@media (min-width: 768px) {
.btn-login{
    margin-left: -10px;
}
}

/* Desktop Version */
@media (min-width: 992px) {

.nav-link:hover::after {
    content: "";
    display: block;
    border-bottom: 2px solid #F85E1D;
    width: 50%;
    margin: auto;
    padding-bottom: 5px;
    margin-bottom: -8px;
}
.navbar-brand, .nav-link, .btn-login{
    color: white !important;
    text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.41);
}
.btn{
    color: white;
    text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.41);
    
} 
.navbar-brand {
    font-size: 36px;
}
}
</style>