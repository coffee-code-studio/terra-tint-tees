<script lang="ts">
    import forestBackground from '$lib/assets/ohio-forest-1.png'
    import terraTintLogo from '$lib/assets/terra-tint-white.png'
</script>

<section
  class="relative bg-cover bg-center bg-no-repeat"
  style={`background-image:url(${forestBackground})`}
>
  <div
    class="absolute inset-0 bg-white/75 sm:bg-transparent sm:from-white/95 sm:to-white/25 sm:bg-gradient-to-r sm:bg-gradient-to-l"
  ></div>

  <div class="relative mx-auto max-w-screen-xl px-4 py-32 sm:px-6 lg:flex lg:h-screen lg:items-center lg:px-8">
    <div class="max-w-xl text-center sm:text-left">
      <h1 class="text-3xl font-extrabold sm:text-5xl">
        Earth-Kind Threads
        <strong class="block font-extrabold text-green-700">Style with a Conscience.</strong>
      </h1>
  
      <p class="mt-4 max-w-lg sm:text-xl">
        Terra Tint: Where style meets sustainability. Our eco-friendly fashion celebrates a love for the planet with every thread.
      </p>
  
      <div class="mt-8 flex flex-wrap gap-4 text-center">
        <a href="/about" class="block w-full rounded bg-green-800 px-12 py-3 text-sm font-medium text-white shadow hover:bg-green-700 focus:outline-none focus:ring active:bg-green-700 sm:w-auto">
          Our Story
        </a>
  
        <a href="/shop" class="block w-full rounded bg-white px-12 py-3 text-sm font-medium text-green-800 shadow hover:text-green-700 focus:outline-none focus:ring active:text-green-700 sm:w-auto">
          Shop
        </a>
      </div>
    </div>
  </div>
</section>