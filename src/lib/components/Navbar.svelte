<script lang="ts">
  import { onMount } from 'svelte'
  import { page } from '$app/stores'
  import { sidebarOpen } from '$lib/stores'
  import terraTintLogo from '$lib/assets/terra-tint-white.png'
  import cartImage from '$lib/assets/cart-shopping-solid-green-edit.png'

  function toggleSidebar() {
    sidebarOpen.update(n => !n)
  }

  function closeSidebar() {
    sidebarOpen.set(false)
  }

  onMount(() => {
    const unsubscribe = page.subscribe(() => {
      closeSidebar()
    })

    return unsubscribe
  })
</script>

<style>
  aside.open {
    transform: translateX(0);
  }
</style>

<!---
<style>
  aside {
    /* Initial sidebar styles (hidden) */
    transform: translateX(-100%);
    transition: transform 0.3s ease;
  }
  aside.open {
    /* Styles when the sidebar is open */
    transform: translateX(0);
  }
</style>
--->

<header class="bg-white">
  <div class="mx-auto max-w-screen-xl px-4 sm:px-6 lg:px-8">
    <div class="flex h-16 items-center justify-between">
      <!-- Left part of the header -->
      <div class="flex-1 md:flex md:items-center md:gap-12">
        <a class="block text-teal-600 dark:text-teal-300" href="/">
          <span class="sr-only">Home</span>
          <img src={terraTintLogo} width={120} height={100} alt="Terra Tint" />
        </a>
      </div>

      <!-- Center navigation for medium and larger screens -->
      <div class="md:flex md:items-center md:gap-12">
        <nav aria-label="Global" class="hidden md:block">
          <ul class="flex items-center gap-6 text-sm">
            <!-- Navigation items here -->
            <li><a class="text-gray-500 transition hover:text-gray-500/75 dark:text-black dark:hover:text-black/75" href="/">Home</a></li>
            <li><a class="text-gray-500 transition hover:text-gray-500/75 dark:text-black dark:hover:text-black/75" href="/about">About</a></li>
            <li><a class="text-gray-500 transition hover:text-gray-500/75 dark:text-black dark:hover:text-black/75" href="/contact">Contact</a></li>
            <li><a class="text-gray-500 transition hover:text-gray-500/75 dark:text-black dark:hover:text-black/75" href="/shop">Shop</a></li>
          </ul>
        </nav>

        <!-- Cart icon -->
        <div class="hidden sm:flex">
          <a href="/cart">
            <img src={cartImage} class="rounded-md bg-gray-50 px-10 py-4 text-sm font-medium text-teal-600 dark:hover:text-white/75" alt="Cart" />
          </a>
        </div>
      </div>

      <!-- Hamburger button for mobile screens -->
      <div class="block md:hidden">
        <button
          class="rounded bg-gray-100 p-2 text-gray-600 transition hover:text-gray-600/75 dark:bg-green-800 dark:text-white dark:hover:text-white/75"
          on:click={toggleSidebar}
        >
          <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</header>

<aside class:open={$sidebarOpen} class="fixed inset-0 w-full bg-white shadow-lg transform translate-x-full transition-transform duration-300 ease-in-out z-50">
  <button class="absolute top-0 right-0 m-4 text-2xl" on:click={closeSidebar}>
    X
  </button>
  <ul class="flex flex-col items-center justify-center h-full space-y-6">
    <li><a href="/" class="text-lg text-gray-700 hover:text-gray-900" on:click={closeSidebar}>Home</a></li>
    <li><a href="/about" class="text-lg text-gray-700 hover:text-gray-900" on:click={closeSidebar}>About</a></li>
    <li><a href="/contact" class="text-lg text-gray-700 hover:text-gray-900" on:click={closeSidebar}>Contact</a></li>
    <li><a href="/shop" class="text-lg text-gray-700 hover:text-gray-900" on:click={closeSidebar}>Shop</a></li>
  </ul>
</aside>