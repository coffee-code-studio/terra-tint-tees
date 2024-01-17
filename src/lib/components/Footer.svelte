<script lang="ts">
    import terraTintLogo from '$lib/assets/terra-tint-white.png'
</script>

<footer class="bg-white">
    <div class="mx-auto max-w-5xl px-4 py-16 sm:px-6 lg:px-8">
      <div class="flex justify-center text-green-600">
        <img src={terraTintLogo} width={200} height={164} alt="Terra Tint" />
      </div>

      <div class="flex justify-center">
        Designed by&nbsp;<a href="https://coffeecodestudio.com/"><strong class="bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 bg-clip-text text-transparent">Coffee Code Studio</strong></a>
      </div>

      <ul class="mt-12 flex flex-wrap justify-center gap-6 md:gap-8 lg:gap-12">
        <li>
          <a class="text-gray-700 transition hover:text-gray-700/75" href="/about">About</a>
        </li>
        <li>
          <a class="text-gray-700 transition hover:text-gray-700/75" href="/contact">Contact</a>
        </li>
  
        <li>
          <a class="text-gray-700 transition hover:text-gray-700/75" href="/shipping">Shipping</a>
        </li>
      </ul>
    </div>
</footer>