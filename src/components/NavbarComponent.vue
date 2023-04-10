<template>
    <div>
        <section class=" top-nav py-2 " >
            <div class="container d-flex justify-content-between align-items-center">
                <div>
                    <span style="padding-right: 10px; color:white;"><a href="" target="_blank" style="color:white; text-decoration:none;">info@gmail.com</a></span>
                </div>
                <div class="text-white d-flex align-items-center">
                    <span><a href="" target="_blank"><i class="fa-brands fa-facebook  text-white"></i> </a></span>
    
                    <span class="mx-2"><a href="" target="_blank"><i class="fa-brands fa-youtube text-white"></i></a></span>
    
                    <span class="ms-2">|</span>
                    <a class="ms-2 btn btn-sm text-white" href="/admin/login" target="black">Login</a>
                </div>
            </div>
        </section>

        <section>

            <nav class="navbar navbar-expand-lg navbar-light bg-light">
                <div class="container">
                  <a class="navbar-brand" href="#"><img src="../assets/Dharan Kitchen.png" alt="" style="height: 45px; "></a>
                  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                  </button>
                  <div class="nav-menu collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#about">Room</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#product">Packages</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#gallery">Dining</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active " aria-current="page" href="#contact">Meeting & Events</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active " aria-current="page" href="#contact">Gallery</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active " aria-current="page" href="#contact">Contact</a>
                        </li>
                        <button class="btn">
                            <a class="ms-2 btn btn-sm " href="/admin/login" target="black">Book Now </a>
                        </button>
                    </ul>
    
                </div>
                </div>
              </nav>
        </section>
    
    </div>
</template>

<script>
    export default {
        name:"NavbarComponent"
    }
</script>

<style  scoped>
.top-nav {
    background: var(--kPrimary);
    height: 40px;
    font-size: 14px;
    transition: all 0.5s;
    color: #fff;
}
.navbar {
    background: #fff;
    transition: all 0.5s;
    z-index: 997;
    box-shadow: 0px 2px 15px rgba(0, 0, 0, 0.1);
}

.nav-menu ul {
    margin: 0;
    padding: 0;
    list-style: none;
}

.nav-menu>ul {
    display: flex;
}

.nav-menu>ul>li {
    position: relative;
    white-space: nowrap;
    padding: 10px 0 10px 28px;
}

.nav-menu a {
    display: block;
    position: relative;
    color: #222222;
    transition: 0.3s;
    font-size: 15px;
    font-weight: 600;
    padding: 0 3px;
    font-family: "Open Sans", sans-serif;
}

.nav-menu>ul>li>a:before {
    content: "";
    position: absolute;
    width: 100%;
    height: 2px;
    bottom: -5px;
    left: 0;
    background-color: var(--kParagraph);
    visibility: hidden;
    width: 0px;
    transition: all 0.3s ease-in-out 0s;
}

.nav-menu a:hover:before,
.nav-menu li:hover>a:before,
.nav-menu .active>a:before {
    visibility: visible;
    width: 100%;
}

.nav-menu a:hover,
.nav-menu .active>a,
.nav-menu li:hover>a {
    color: var(--kParagraph);
}
.btn{
    background-color: var(--acent)
}
</style>