<script lang="ts">
  const stats = [
    {
      label: "$2.5B+",
      desc: "In total transaction value across food and agribusiness deals. Our track record spans craft beverages, specialty ingredients, protein processing, organic foods, and agricultural services—delivering successful outcomes across the entire value chain.",
      img: "/generated/image-professional-business-advisor-in-suit-wi-1765564765758-0.webp"
    },
    {
      label: "50+ Transactions",
      desc: "Successfully closed deals ranging from $10M to $200M+ in enterprise value. Each transaction represents a business owner's life work, and we treat it with the respect and dedication it deserves.",
      img: "/generated/image-stack-of-signed-business-documents-and-c-1765564768860-1.webp"
    },
    {
      label: "15+ Years",
      desc: "Of specialized focus on food and agribusiness M&A. Our team brings decades of combined experience from leading investment banks, operating companies, and advisory firms—all dedicated to this sector.",
      img: "/generated/image-vintage-clock-or-hourglass-representing--1765564771165-2.webp"
    },
    {
      label: "100% Success Rate",
      desc: "Every engagement we accept reaches a successful close. We're selective about the clients we work with, ensuring we can deliver exceptional results. When we commit to your transaction, we see it through to completion.",
      img: "/generated/image-handshake-between-business-professionals-1765564926113-0.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Our track record speaks to our commitment and expertise in food and agribusiness M&A.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
