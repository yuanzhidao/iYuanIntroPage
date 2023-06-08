<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header class="snap-start snap-always">
    <div class="drawer lg:hidden">
      <input id="drawer-1" type="checkbox" class="drawer-toggle" />
      <div class="drawer-content flex flex-col">
        <!-- Navbar -->
        <div class="w-full navbar bg-base-100">
          <div class="flex-1 lg:hidden">
            <label for="drawer-1" class="btn btn-square btn-ghost">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-5 h-5 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
            </label>
          </div>
          <div class="flex-none hidden lg:block">
            <ul class="menu menu-horizontal">
              <li><RouterLink to="/">主页</RouterLink></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="drawer-side">
        <label for="drawer-1" class="drawer-overlay"></label>
        <ul class="menu p-4 w-[14rem] h-full bg-base-200">
          <!-- Sidebar content here -->
          <li>
            <RouterLink to="/"
              ><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
              </svg>
              主页</RouterLink
            >
          </li>
        </ul>
      </div>
    </div>
  </header>

  <RouterView />

  <footer class="snap-start snap-always">
    <div class="font-light text-zinc-500 p-4 mt-8 mb-[10rem]">
      <p>2023 © iYuan</p>
      <a href="https://beian.miit.gov.cn" class="hover:underline">沪ICP备2022026478号-3</a>
    </div>
  </footer>
</template>
