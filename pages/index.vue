<template>
  <div class="bg-[url(@/static/img/hero.png)] bg-[center] bg-no-repeat bg-cover z-0">
    <section class="hero pt-[107px]">
      <div class="container">
        <div class="flex justify-between">
          <div class="hero-links flex flex-col justify-between">
            <nuxt-link to="/Изыскания" class="text-[#4F4747] text-[24px] montserrat">Изыскания</nuxt-link>
            <nuxt-link to="/Обследование" class="text-[#4F4747] text-[24px] montserrat">Обследование</nuxt-link>
            <nuxt-link to="/Проектирование" class="text-[#4F4747] text-[24px] montserrat">Проектирование</nuxt-link>
            <nuxt-link to="/Геотехника" class="text-[#4F4747] text-[24px] montserrat">Геотехника</nuxt-link>
            <nuxt-link to="/Исследования" class="text-[#4F4747] text-[24px] montserrat">Исследования</nuxt-link>
          </div>
          <div class="w-[80%] max-h-[407px] bg-[#D9D9D980]">
            <video src="" class="w-[100%] h-[100%]"></video>
          </div>
        </div>
      </div>
    </section>
    <section class="news mt-[36px] h-[371px]">
      <div class="container bg-[#D9D9D980] h-full p-[40px]">
        <div class="title">
          <h2 class="text-[#4F4747] text-[32px] montserrat font-semibold">Новости</h2>
        </div>
      </div>
    </section>
    <section class="vacancies mt-[36px] h-[468px] mb-[38px]">
      <div class="container bg-[#D9D9D980] h-full p-[40px]">
        <div class="title">
          <h2 class="text-[#4F4747] text-[32px] montserrat font-semibold">Вакансии</h2>
        </div>
      </div>
    </section>
    <div class="w-full h-[7px] line"></div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>

.line {
  background: linear-gradient(90deg, #FD7F02 12.08%, #5B5B5B 54.14%, #0001F9 94.48%);;
}

</style>
