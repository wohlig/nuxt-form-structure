<template>
  <div class="Header header header-1 bgcover" >
        <div class="container">
            <b-navbar toggleable="lg" type="dark">
                <b-navbar-brand href="/" >
                    <img src="~/assets/Images/logo-wohlig.png" alt="Wohlig">
                </b-navbar-brand>
                <b-navbar-toggle target="nav-collapse"><span aria-hidden="true" class="icon_menu hamb-mob-icon "></span></b-navbar-toggle>
                <b-collapse id="nav-collapse" is-nav>
                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto font-montserrat ">
                    <b-navbar-nav  v-for="nav in Navigations" v-bind:key="nav.index"
                            :to="nav.to">
                        <b-nav-item class="current">{{nav.title}}</b-nav-item>
                    </b-navbar-nav>
                </b-navbar-nav>
                </b-collapse>
            </b-navbar>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            Navigations:[
                {
                    link:"#Home",
                    title:"Home",
                    to: '/'

                },
                 {
                    link:"#about-us",
                    title:"About Us",
                    to: '/about-us'
                },
                 {
                    link:"#services",
                    title:"Services",
                    to: '/services'
                },
                 {
                    link:"#work-process",
                    title:"Work Process",
                    to: '/work-process'
                },
                 {
                    link:"#clients",
                    title:"Clients",
                    to: '/clients'
                },
                {
                    link:"#contact-us",
                    title:"Contact",
                    to: '/contact-us'
                }
            ]
        }
    },



}
</script>

<style>
.navbar-dark .navbar-nav .nav-link {
    color:#323336;
    font-size: 17px;
    padding: 22px;
}
.navbar-brand>img{
    height: 42px;
}
.navbar-dark .navbar-nav .nav-link:hover{
    color: #323336;
}
.navbar-dark .navbar-nav .nav-link:focus{
    color: #fff;
}
.navbar-dark .navbar-toggler {
    color: #323336;
    border-color: #323336;
}
.navbar-dark .navbar-toggler {
    color: #323336;
    border:0;
}
button:focus{
    outline: 0;
}
@media (max-width: 1024px){
.hamb-mob-icon {
    padding: 0px;
    }
.main-menu-container{
    background-image: linear-gradient( to right,rgba(48,172,177,1),rgba(115,173,39,1) );
}
.bgcover{
    box-shadow: none;
}
}
</style>
