<script>
    // Svelte script section for handling any reactive logic
  </script>
  
  <style>
    /* Additional CSS styles if needed */
  </style>
  
  <div class="container mx-auto px-4 mt-40">
      <h1 class="text-2xl font-bold my-4 text-5xl">Shipping</h1>
  
      <div>
          <p>Orders are typically processed within 1-2 business days. This time may increase during November and December. We utilize USPS and UPS for shipping orders within the US.</p>
          <!-- Shipping Options Table -->
          <table class="min-w-full leading-normal mt-4">
              <thead>
                  <tr>
                      <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-600 uppercase tracking-wider">Shipping Option</th>
                      <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-600 uppercase tracking-wider">Order Total</th>
                      <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-600 uppercase tracking-wider">Shipping Cost</th>
                  </tr>
              </thead>
              <tbody>
                  <tr>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">Standard Shipping</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">$75+</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">Free</td>
                  </tr>
                  <tr>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">International Shipping</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">All Orders</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">Variable</td>
                  </tr>
              </tbody>
          </table>
          <p class="mt-4">International orders may be subject to additional duties. We offer the option to prepay duties so there are no surprises upon delivery.</p>
      </div>
  
      <div class="mt-8">
          <h2 class="text-xl font-bold my-4">Returns & Exchanges</h2>
          <p>We accept returns and exchanges for items that are unworn and unwashed within 30 days of purchase.</p>
  
          <ul class="list-disc pl-5 mt-4">
              <li>Drop your item off at a Happy Returns Bar. We'll show you the closest location, or you can check here. This is an eco-friendly, label-free and packaging-free option.</li>
              <li>Mail your return. Print a label and affix it to the original packaging with the return items inside.</li>
          </ul>
      </div>
  
      <div class="mt-8">
          <h2 class="text-xl font-bold my-4">Our Cost of Returns Transparency</h2>
          <!-- Cost of returns table -->
          <table class="min-w-full leading-normal mt-4">
              <thead>
                  <tr>
                      <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-600 uppercase tracking-wider">Cost per Item</th>
                      <th class="px-5 py-3 border-b-2 border-gray-200 bg-gray-100 text-left text-xs font-semibold text-gray-600 uppercase tracking-wider">Description</th>
                  </tr>
              </thead>
              <tbody>
                  <tr>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">$5.75</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">Return Shipping</td>
                  </tr>
                  <tr>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">$1.25</td>
                      <td class="px-5 py-5 border-b border-gray-200 bg-white text-sm">Return Confirmation, Organization, and 3-Point Inspection</td>
                  </tr>
                  <!-- Additional rows as needed -->
              </tbody>
          </table>
          <p class="mt-4">We charge $7.99 per item returned for a refund. Exchanges are free. Returns for store credit are free.</p>
      </div>
  
      <div class="mt-8">
          <h2 class="text-xl font-bold my-4">International Returns</h2>
          <p>International customers are responsible for return shipping costs, and duties are not refundable. International exchanges are not currently supported. Please email contact@happyearthapparel.com to start the return process.</p>
          <!-- 'Start a Return' button -->
          <button class="mt-4 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
              <a href="/returns">Start a Return</a>
          </button>
      </div>
  </div>
  