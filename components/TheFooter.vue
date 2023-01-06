<template>
    <footer class="bg-[#1C2752]">
        <div class="container flex justify-between items-center py-[144px] flex-wrap">
            <div class="footer-other-links">
                <div class="footer-other-links__title flex justify-between gap-[19px]">
                    <img src="@/static/img/Logo.svg" alt="logo" class="w-[91px] h-[55px]">
                    <div class="flex justify-between flex-col h-[55px] text-[17px] text-white">
                        <p>OOO</p>
                        <p>“Geofundamentproject”</p>
                    </div>
                </div>
                <div class="socialMedia flex justify-between items-center gap-[20px] mt-[50px] mb-[49px]">
                    <div
                        class="socialMedia__item w-[60px] h-[60px] bg-[#2C3765] rounded-[100px] flex justify-center items-center">
                        <img src="@/static/img/inst.svg" alt="inst">
                    </div>
                    <div
                        class="socialMedia__item w-[60px] h-[60px] bg-[#2C3765] rounded-[100px] flex justify-center items-center">
                        <img src="@/static/img/tg.svg" alt="tg">
                    </div>
                    <div
                        class="socialMedia__item w-[60px] h-[60px] bg-[#2C3765] rounded-[100px] flex justify-center items-center">
                        <img src="@/static/img/facebook.svg" alt="facebook">
                    </div>
                    <div
                        class="socialMedia__item w-[60px] h-[60px] bg-[#2C3765] rounded-[100px] flex justify-center items-center">
                        <img src="@/static/img/youtube.svg" alt="youtube">
                    </div>
                </div>
                <div class="signature text-[10px] text-white">
                    <p>© Desinger by Limbo</p>
                </div>
            </div>
            <div class="footer-links">
                <div class="footer-links__title text-white text-[25px] mb-[38px]">
                    <h3>Навигация</h3>
                </div>
                <div class="footer-links__links flex justify-between gap-[56px]">
                    <div class="flex flex-col justify-between gap-[20px]">
                        <nuxt-link to="/footer" class="text-white text-[18px]">Главная</nuxt-link>
                        <nuxt-link to="/footer" class="text-white text-[18px]">О компании</nuxt-link>
                        <nuxt-link to="/footer" class="text-white text-[18px]">Услуги</nuxt-link>
                    </div>
                    <div class="flex flex-col justify-between gap-[20px]">
                        <nuxt-link to="/footer" class="text-white text-[18px]">Наши проекты</nuxt-link>
                        <nuxt-link to="/footer" class="text-white text-[18px]">Наши достижение</nuxt-link>
                        <nuxt-link to="/footer" class="text-white text-[18px]">Контакты</nuxt-link>
                    </div>
                </div>
            </div>
            <div class="connect flex flex-col justify-between gap-[20px]">
                <a href="#" class="connect__item flex gap-[17px]">
                    <div class="bg-[#F9B44E] py-[24px] px-[26px] rounded-[100px]">
                        <img src="@/static/img/mail.svg" alt="mail">
                    </div>
                    <div class="flex flex-col justify-between">
                        <p class="text-[20px] text-white">Mail Us</p>
                        <p class="text-[17px] text-white">uzssmge.com</p>
                    </div>
                </a>
                <a href="#" class="connect__item flex gap-[17px]">
                    <div class="bg-[#F9B44E] py-[24px] px-[26px] rounded-[100px]">
                        <img src="@/static/img/phone.svg" alt="[phone]">
                    </div>
                    <div class="flex flex-col justify-between">
                        <p class="text-[20px] text-white">Call Us</p>
                        <p class="text-[17px] text-white">+998 97 923 33 73</p>
                    </div>
                </a>
                <a href="#" class="connect__item flex gap-[17px]">
                    <div class="bg-[#F9B44E] py-[24px] px-[26px] rounded-[100px]">
                        <img src="@/static/img/location.svg" alt="location">
                    </div>
                    <div class="flex flex-col justify-between">
                        <p class="text-[20px] text-white">Location</p>
                        <p class="text-[17px] text-white">Лолазор, 73</p>
                    </div>
                </a>
            </div>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>

<style>

</style>