<script lang="ts">
  const sectors = [
    "Craft Beverages",
    "Specialty Foods",
    "Organic Products",
    "Protein Processing",
    "Food Ingredients",
    "Agricultural Services",
    "Distribution",
    "Food Manufacturing"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-black via-gray-800 to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#000_0%,#1a1a1a_30%,#4a4a4a_60%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      Connecting Food & Agribusiness Owners to Strategic Buyers. <span class="text-gray-300">We deliver specialized middle market M&A expertise, guiding you from valuation to close with proven industry relationships.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8">
    <p class="text-xs uppercase tracking-wider text-gray-400 mb-4">Sectors We Serve</p>
    <div class="flex flex-wrap gap-4 md:gap-6 items-center">
      {#each sectors as sector}
        <div class="text-sm text-gray-500 font-medium">{sector}</div>
      {/each}
    </div>
  </div>
</section>
