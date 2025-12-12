<script lang="ts">
  const cards = [
    {
      title: "We're Not Just Advisors...",
      subtitle: "We're Your Trusted Partners.",
      image: "/generated/image-professional-business-meeting-with-execu-1765563982899-0.webp"
    },
    {
      title: "We Don't Just Know Finance...",
      subtitle: "We Know Food & Agribusiness.",
      image: "/generated/image-agricultural-landscape-with-modern-farmi-1765563985699-1.webp"
    },
    {
      title: "We Don't Just Close Deals...",
      subtitle: "We Maximize Your Legacy.",
      image: "/generated/image-business-handshake-between-executives-in-1765563988233-2.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Your exit is one of the most important decisions you'll ever make. We're not here to push a quick transaction—we're here to understand your goals, protect your interests, and deliver outcomes that honor what you've built.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
