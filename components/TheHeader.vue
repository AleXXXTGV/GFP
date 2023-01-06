<template>
    <header class="header  xl:bg-[#1C2752]">
        <div class="mobile-menu xl:hidden" :class="{ mobile_menu_active: showMobileMenu == true }">
            <nav class="links">
                <nuxt-link to="/" class="link">Главная</nuxt-link>
                <nuxt-link to="/about" class="link">О компании</nuxt-link>
                <nuxt-link to="/services" class="link">Услуги</nuxt-link>
                <nuxt-link to="/projects" class="link">Наши проекты</nuxt-link>
                <nuxt-link to="/progress" class="link">Наши достижение</nuxt-link>
                <nuxt-link to="/events" class="link">События</nuxt-link>
                <nuxt-link to="/contacts" class="link">Контакты</nuxt-link>
            </nav>
            <div class="languages">
                <div class="language">
                    <img src="@/static/img/en.svg" alt="EN">
                    <p>EN</p>
                </div>
                <div class="language">
                    <img src="@/static/img/ru.svg" alt="RU">
                    <p>RU</p>
                </div>
                <div class="language">
                    <img src="@/static/img/uz.svg" alt="UZ">
                    <p>UZ</p>
                </div>
            </div>
        </div>
        <div class="container flex justify-between items-center xl:hidden">
            <div class="header-mobile__logo">
                <img src="@/static/img/Logo.svg" alt="logo">
            </div>
            <div class="toggle xl:hidden flex" :class="{ active: showMobileMenu == true }"
                @click="showMobileMenu = !showMobileMenu">
                <span></span>
                <span></span>
                <span></span>
            </div>

        </div>
        <div class="container header-container hidden justify-between items-center py-[10px] xl:flex">
            <div class="w-[102px] h-[64px]">
                <img src="@/static/img/Logo.svg" alt="logo">
            </div>
            <nav class="w-[70%] flex justify-between items-center">
                <nuxt-link to="/" class="text-white pb-[5px] font-bold montserrat">Главная</nuxt-link>
                <nuxt-link to="/about" class="text-white pb-[5px] font-bold montserrat">О компании</nuxt-link>
                <nuxt-link to="/services" class="text-white pb-[5px] font-bold montserrat">Услуги</nuxt-link>
                <nuxt-link to="/projects" class="text-white pb-[5px] font-bold montserrat">Наши проекты</nuxt-link>
                <nuxt-link to="/progress" class="text-white pb-[5px] font-bold montserrat">Наши достижение</nuxt-link>
                <nuxt-link to="/events" class="text-white pb-[5px] font-bold montserrat">События</nuxt-link>
                <nuxt-link to="/contacts" class="text-white pb-[5px] font-bold montserrat">Контакты</nuxt-link>
            </nav>
            <div class="flex justify-between items-center gap-[2px]">
                <nuxt-link to="/ru" class="text-white pb-[5px] font-normal montserrat">РУ</nuxt-link>
                <span class="text-white pb-[5px] font-normal montserrat">|</span>
                <nuxt-link to="/en" class="text-white pb-[5px] font-normal montserrat">EN</nuxt-link>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'TheHeader',
    data() {
        return {
            showMobileMenu: false,
        };
    },
}
</script>

<style>
.header {
    width: 100%;
    position: fixed;
}

/* .header-container {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-top: 30px;
    position: relative;
} */

.header-mobile {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.header-mobile__logo {
    width: 75px;
    height: 45px;
}

/* .header-mobile__burger {
    width: 40px;
    height: 16px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.burger-line {
    width: 100%;
    height: 2px;
    background-color: #FCFCFC;
    border-radius: 100px;
} */

.toggle {
    position: relative;
    width: 70px;
    height: 70px;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    overflow: hidden;
    z-index: 3;
}

.toggle span {
    position: absolute;
    width: 40px;
    height: 2px;
    background: #FCFCFC;
    border-radius: 4px;
    transition: 0.5s;
}

.toggle span:nth-child(1) {
    transform: translateY(-15px);
    width: 25px;
    left: 15px;
}

.toggle.active span:nth-child(1) {
    width: 40px;
    transform: translateY(0px) rotate(45deg);
    transition-delay: 0.125s;
    background-color: #3C3C3C;
}

.toggle span:nth-child(2) {
    transform: translateY(15px);
    width: 15px;
    left: 15px;
}

.toggle.active span:nth-child(2) {
    width: 40px;
    transform: translateY(0px) rotate(315deg);
    transition-delay: 0.125s;
    background-color: #3C3C3C;
}

.toggle.active span:nth-child(3) {
    transform: translateX(60px);
    background-color: #3C3C3C;
}

.mobile-menu {
    background-color: white;
    position: absolute;
    top: -700%;
    left: 0;
    width: 100%;
    height: 100vh;
    display: flex;
    opacity: 0;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    z-index: 2;
    padding-top: 86.5px;
    transition: 700ms ease;
}

.mobile_menu_active {
    opacity: 1;
    top: 0;
}

.links {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    height: 66%;
}

.link {
    color: black;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 27px;
}

.nuxt-link-active {
    color: orange;
}

.languages {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 90%;
    gap: 3px;
}

.language {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
</style>