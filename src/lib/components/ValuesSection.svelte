<script lang="ts">
  const photos = [
    {
      title: "Industry Expertise",
      desc: "Our team has deep operational experience in food and agribusiness, understanding the unique challenges and opportunities in this sector.",
      img: "/generated/image-professional-business-advisor-consulting-1765563990528-3.webp"
    },
    {
      title: "Strategic Relationships",
      desc: "We maintain active relationships with strategic buyers, private equity firms, and family offices focused on food and agribusiness investments.",
      img: "/generated/image-group-of-business-professionals-networki-1765563992933-4.webp"
    },
    {
      title: "Proven Process",
      desc: "Our disciplined approach combines financial rigor with strategic positioning, ensuring every transaction achieves maximum value for our clients.",
      img: "/generated/image-business-team-analyzing-financial-charts-1765563995369-5.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">Why business owners choose Westerra Capital</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      We're not generalists trying to cover every industry. Our exclusive focus on food and agribusiness means we know the buyers, understand the market dynamics, and can position your business for maximum value.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
