<template>
    <nav>

        <input class="menu-btn" type="checkbox" id="menu-btn">
        <label class="menu-icon" for="menu-btn">
            <font-awesome-icon icon="bars" class="nav-icon"/>
        </label>

        <ul class="menu" >
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#about">Sobre mi</a></li>
            <li><a href="#servicios">Servicios</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#estudios">Estudios</a></li>
            <li><a href="#trabajo">Trabajo</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>

    </nav>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@200&family=Overlock&display=swap');

ul {
    list-style: none;
}

a {
    text-decoration: none;
}

#main {
    width: 40%;
    height: 100vh;
    position: relative;
}

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    box-shadow: 5px 10px 30px rgba(0,0,0, 0.02);
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    z-index: 1;
    background-color: black;
}


nav ul {
    display: flex;
    width: 90%;
    justify-content: center;
}

nav ul li {
    height: 40px;
    line-height: 55px;
    margin: 10px;
    padding: 0px 22px;
    text-transform: uppercase;
    text-align: center;
    font-weight: 500;
    color: #585b5b;
    letter-spacing: 1px;
}

nav ul li a {
    color: white;
    font-size: 0.78rem;
}

nav ul li a:hover {
    color: #9d9ce3;
}

@media (min-width: 999px) {
    nav .menu-icon {
        display: none;
    }

    nav .menu-btn {
        display: none;
    }

    nav ul li {
        
        display: flex;
    }
        
}

@media (max-width: 998px) {

    nav {
        justify-content: space-between;
        height: 80px;
        padding: 0px 30px;
    }

    .logo img {
        height: 30px;
    }

    .menu {
        display: none;
        position: absolute;
        top: 65px;
        left: 0px;
        background-color: black;
        border-bottom: 4px solid #9d9ce3;
        width: 100%;
        height: 410px;
        padding: 0px;
        margin: 0px;
    }

    .menu li {
        width: 100%;
    }

    nav .menu li a{
        width: 100%;
        height: 40px;
        justify-content: center;
        align-items: center;
        margin: 0px;
        padding: 25px;
        border: 1px solid rgba(38, 38, 38, 0.03);
        cursor: pointer;
    }

    nav .menu-icon {
        float: right;
        padding: 28px 20px;
        position: relative;
        user-select: none;
    }

    nav .menu-icon .nav-icon {
        display: block;
        height: 23px;
        position: relative;
        transition: background 0.2s ease-out;
        width: 23px;
        color: white;
    }
    
    nav .menu-icon .nav-icon:before,
    nav .menu-icon .nav-icon:after {
        background: white;
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all ease-out 0.2s;
    }

    nav .menu-icon .nav-icon:before {
        top: 5px;
    }

    nav .menu-icon .nav-icon:after {
        top: -5px;
    }

    nav .menu-btn:checked ~ .menu-icon .nav-icon {
        background:  transparent;
    }
    
    nav .menu-btn:checked ~ .menu-icon .nav-icon:before {
        transform: rotate(-45deg);
        top: 0;
    }

    nav .menu-btn:checked ~ .menu-icon .nav-icon:after {
        transform: rotate(45deg);
        top: 0;
    }

    nav .menu-btn {
        display: none;
    }

    nav .menu-btn:checked ~ .menu {
        display: block;
    }

}

</style>