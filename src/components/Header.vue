<script>
export default {};
</script>

<template>
  <div class="container mx-auto">
    <div class="flex justify-between items-end py-5">
      <div class="flex items-center gap-8">
        <img
          class=" p-5"
          src="/images/Каталог бургер.svg"
          alt=""
        />
        <img src="/images/Лого.svg" alt="" />
      </div>
      <nav>
        <ul class="flex gap-5 mb-6">
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
        <form action="" class="flex relative">
          <select
            class="text-base font-light focus:outline-none bg-gradient-to-r from-purple-500/10 to-pink-500/10 absolute py-2 px-3 top-1 left-1"
            name=""
            id=""
          >
            <option value="">Везде</option>
          </select>
          <input
            type="text"
            class="min-w-[700px] px-28 gradient-border border border-gradien py-2 focus:outline-none"
          />
          <img class="absolute right-5 top-2" src="/images/search.png" alt="" />
        </form>
      </nav>
      <div class="">
        <div
          class="flex font-light divide-x-2 divide-black text-xs justify-end mb-6"
        >
          <img class="px-2" src="/images/Flag Ru.svg" alt="" />
          <p class="px-2">Русский</p>
          <select class="focus:outline-none bg-white" name="" id="">
            <option value="">₽</option>
          </select>
        </div>
        <div class="flex text-center text-sm gap-14">
          <span class="text-center">
            <img class="mx-auto mb-1" src="/images/user.png" alt="" />
            <p>Войти</p>
          </span>
          <span class="text-center">
            <img class="mx-auto mb-1" src="/images/like-heart.svg" alt="" />
            <p>Избранное</p>
          </span>
          <span class="text-center">
            <img class="mx-auto mb-1" src="/images/cart.svg" alt="" />
            <p>Корзина</p>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>