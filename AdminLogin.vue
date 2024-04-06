<template>
  <img
    class="fixed top-0 left-0 right-0 bottom-0 w-full h-full z-0"
    src="../../assets/images/la.jpeg"
    alt=""
  />
  <div class="relative z-1 flex justify-center items-center">
    <div class="w-1/3 h-[450px] bg-slate-700 rounded-xl">
      <div class="w-full h-full px-10 py-10">
        <div class="text-xl mb-5">Welcome to <span class="font-bold">Move Admin</span></div>
        <form class="">
          <label class="text-base cursor-pointer block my-3" for="email">Email</label>
          <input
            class="input-login-signup w-full h-[40px] rounded-lg pl-4"
            type="email"
            id="email"
          />
          <label class="text-base cursor-pointer block my-3" for="password">Password</label>
          <input class="input-login-signup w-full h-[40px] rounded-lg" type="text" id="password" />
          <button
            class="flex justify-center items-center w-full h-12 mt-10 bg-[#999999] text-[#cccc] rounded-[10px] font-bold text-[16px]"
            :class="{ '!bg-[#13D0B4] text-white': isAllInputFilled }"
          >
            Submit
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped></style>
