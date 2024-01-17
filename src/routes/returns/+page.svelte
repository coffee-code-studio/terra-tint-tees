<script lang="ts">
    let showError = false
  
    function toggleError() {
      showError = !showError
    }
    //
</script>

<div class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 flex flex-col">
    <div class="mb-4">
      <h1 class="text-lg font-semibold text-gray-700 mt-40 text-5xl">Terra Tint</h1>
    </div>
    
    <div class="mb-6">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="order-number">
        Order Number/ID
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="order-number" type="text" placeholder="HEA12345">
    </div>
  
    <div class="mb-6">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="zip-code">
        Zip/Postal Code
      </label>
      <input class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" id="zip-code" type="text" placeholder="Zip/Postal Code">
    </div>
  
    <div class="flex flex-col sm:flex-row items-center justify-between space-y-2 sm:space-y-0 sm:space-x-2">
        <button
          class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline w-full sm:w-auto"
          on:click={toggleError}
          type="button"
        >
          Start Your Return
        </button>
        <a
          class="inline-block align-baseline font-bold text-sm text-blue-500 hover:text-blue-800 cursor-pointer w-full sm:w-auto text-center"
          on:click={toggleError}
        >
          Received a gift? Start Here
        </a>
      </div>
</div>

{#if showError}
  <div class="text-red-500 text-sm mt-2">
    An error occurred, please try again.
  </div>
{/if}
  