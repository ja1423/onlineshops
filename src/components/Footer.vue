<template>
  <div class="container mx-auto bg-gradient-to-t from-[#F64D4D] to-[#4D5EF6] py-8 md:py-12">
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 md:gap-8 mx-4 md:mx-8">
      <div class="border-b pb-4 md:pb-0">
        <h1 class="text-xl md:text-2xl font-bold mb-4 md:mb-6">Покупателям</h1>
        <ul class="text-sm md:text-base">
          <li><a class="hover:text-[#46A358]" href="#">Как это работает</a></li>
          <li><a class="hover:text-[#46A358]" href="#">Защита покупателя</a></li>
          <li><a class="hover:text-[#46A358]" href="#">Условия оплаты</a></li>
          <li><a class="hover:text-[#46A358]" href="#">Условия использования</a></li>
          <li><a class="hover:text-[#46A358]" href="#">Регистрация аккаунта</a></li>
        </ul>
      </div>
      <!-- Repeat the same structure for other sections -->
    </div>
    <div class="flex flex-col items-center justify-center mt-6 md:mt-10">
      <h2 class="text-lg md:text-xl font-bold mb-3">Хотите быть в курсе последних новостей и акций?</h2>
      <div class="flex gap-4">
        <img class="h-8 md:h-10" src="/icons/w.svg" alt="WhatsApp" />
        <img class="h-8 md:h-10" src="/icons/instagram.svg" alt="Instagram" />
        <img class="h-8 md:h-10" src="/icons/facebook.svg" alt="Facebook" />
      </div>
    </div>
    <p class="text-center mt-6 text-sm text-[#3D3D3D]">&copy; PlaceMik.ru, 2021</p>
  </div>
</template>

<script>
export default {};
</script>

<style scoped></style>
