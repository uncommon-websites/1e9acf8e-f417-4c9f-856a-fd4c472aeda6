<script lang="ts">
  const projects = [
    {
      client: "Artisan Beverage Co.",
      desc: "Successfully positioned craft beverage company for strategic acquisition by regional distributor.",
      bg: "bg-black",
      img: "/generated/image-craft-brewery-production-facility-with-s-1765564303508-0.webp",
      dark: true
    },
    {
      client: "Heritage Foods Group",
      desc: "Navigated complex family succession through strategic sale to private equity.",
      bg: "bg-gray-200",
      img: "/generated/image-modern-food-processing-facility-with-wor-1765564305994-1.webp",
      dark: false
    },
    {
      client: "Organic Valley Processors",
      desc: "Maximized valuation in competitive auction process with multiple strategic buyers.",
      bg: "bg-gray-100",
      img: "/generated/image-organic-farm-with-fresh-vegetables-and-g-1765564308325-2.webp",
      dark: false
    },
    {
      client: "Premium Protein Partners",
      desc: "Structured innovative earn-out agreement securing optimal terms for sellers.",
      bg: "bg-[#1a1a1a]",
      img: "/generated/image-protein-processing-plant-with-modern-ind-1765564311007-3.webp",
      dark: true
    },
    {
      client: "Midwest Grain Cooperative",
      desc: "Facilitated merger creating leading regional agribusiness platform.",
      bg: "bg-[#f0f0f0]",
      img: "/generated/image-wide-view-of-grain-silos-and-agricultura-1765564313438-4.webp",
      dark: false,
      full: true
    },
    {
      client: "Specialty Ingredients Inc.",
      desc: "Connected niche food ingredient manufacturer with international strategic buyer.",
      bg: "bg-gray-100",
      img: "/generated/image-food-ingredients-laboratory-with-scienti-1765564316008-5.webp",
      dark: false
    },
    {
      client: "Farm Fresh Distribution",
      desc: "Advised on transformational acquisition expanding market reach and capabilities.",
      bg: "bg-gray-200",
      img: "/generated/image-modern-food-processing-facility-with-wor-1765564305994-1.webp",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="mb-4">
    <p class="text-xs uppercase tracking-wider text-gray-400">Select Transactions</p>
  </div>
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We connect food and agribusiness owners with the right buyers</span> through deep industry expertise, proven transaction experience, and relationships that unlock maximum value.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
