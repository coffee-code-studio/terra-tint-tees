<script lang="ts">
  export let imageUrl = ''
  export let customText = ''

  export let outOfStock: any

  function handleAddToCart() {
    outOfStock = true
  }
</script>

<a href="#" class="group relative block overflow-hidden">
    <button
      class="absolute end-4 top-4 z-10 rounded-full bg-white p-1.5 text-gray-900 transition hover:text-gray-900/75"
    >
      <span class="sr-only">Wishlist</span>
    </button>

    <img
      src={imageUrl}
      alt=""
      class="h-80 w-full object-cover transition duration-500 group-hover:scale-105 sm:h-[30rem]"
    />

    <div class="relative border border-gray-100 bg-white p-6">

      <h3 class="mt-4 text-lg font-medium text-gray-900">{customText}</h3>

      {#if outOfStock}
        <p class="text-red-500">Out of Stock</p>
      {/if}

      <p class="mt-1.5 text-sm text-gray-700">$45.00</p>

      <form class="mt-4">
        <button
          class="block w-full rounded bg-green-800 p-4 text-sm text-white font-medium transition hover:scale-105"
          on:click|preventDefault={handleAddToCart}
          disabled={outOfStock}
        >
          Add to Cart
        </button>
      </form>
    </div>
</a>