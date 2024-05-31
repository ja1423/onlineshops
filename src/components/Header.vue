<script>
export default {};
</script>

<template>
  <div class="container mx-auto px-4">
    <div class="flex flex-col lg:flex-row justify-between items-end py-5">
      <div class="flex flex-col lg:flex-row items-center gap-4 lg:gap-8">
        <img class="p-3 lg:p-5 w-16 lg:w-auto" src="/images/Каталог бургер.svg" alt="" />
        <img class="w-24 lg:w-auto" src="/images/Лого.svg" alt="" />
      </div>
      <nav class="w-full lg:w-auto">
        <ul class="flex flex-col lg:flex-row gap-4 lg:gap-5 mb-4 lg:mb-6">
          <li class="font-light text-xs">
            <select class="focus:outline-none bg-white" name="" id="">
              <option value="">Покупателям</option>
            </select>
          </li>
          <li class="font-light text-xs">
            <select class="focus:outline-none bg-white" name="" id="">
              <option value="">Поставщикам</option>
            </select>
          </li>
          <li class="font-light text-xs"><a href="#">Частые вопросы</a></li>
        </ul>
        <form action="" class="flex relative w-full lg:w-auto">
          <select class="text-base font-light focus:outline-none bg-gradient-to-r from-purple-500/10 to-pink-500/10 absolute py-2 px-3 top-1 left-1" name="" id="">
            <option value="">Везде</option>
          </select>
          <input type="text" class="w-full lg:min-w-[700px] px-14 lg:px-28 gradient-border border border-gradient py-2 focus:outline-none" />
          <img class="absolute right-5 top-2" src="/images/search.png" alt="" />
        </form>
      </nav>
      <div class="mt-4 lg:mt-0 w-full lg:w-auto">
        <div class="flex font-light divide-x-2 divide-black text-xs justify-center lg:justify-end mb-4 lg:mb-6">
          <img class="px-2" src="/images/Flag Ru.svg" alt="" />
          <p class="px-2">Русский</p>
          <select class="focus:outline-none bg-white" name="" id="">
            <option value="">₽</option>
          </select>
        </div>
        <div class="flex text-center text-sm gap-6 lg:gap-14 justify-center lg:justify-end">
          <span class="text-center">
            <img class="mx-auto mb-1 w-6 lg:w-auto" src="/images/user.png" alt="" />
            <p>Войти</p>
          </span>
          <span class="text-center">
            <img class="mx-auto mb-1 w-6 lg:w-auto" src="/images/like-heart.svg" alt="" />
            <p>Избранное</p>
          </span>
          <span class="text-center">
            <img class="mx-auto mb-1 w-6 lg:w-auto" src="/images/cart.svg" alt="" />
            <p>Корзина</p>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped></style>