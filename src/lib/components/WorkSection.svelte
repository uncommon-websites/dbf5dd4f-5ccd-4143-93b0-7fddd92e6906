<script lang="ts">
  const projects = [
    {
      client: "American Bitcoin",
      desc: "NASDAQ debut website that positions a Bitcoin company for public markets.",
      bg: "bg-[#0a0a0a]",
      img: "/generated/image-modern-fintech-website-interface-on-lapt-1765564944489-0.webp", 
      dark: true
    },
    {
      client: "XFX",
      desc: "Growth-stage website supporting a $9.1M seed round for a tech startup.",
      bg: "bg-gray-100",
      img: "/generated/image-sleek-fintech-dashboard-interface-on-mul-1765565084744-4.webp",
      dark: false
    },
    {
      client: "Rare Origins",
      desc: "Sophisticated web presence for a single-family investment firm.",
      bg: "bg-[#1a1a1a]",
      img: "/generated/image-elegant-investment-firm-website-on-deskt-1765564947280-1.webp",
      dark: true
    },
    {
      client: "Flychain",
      desc: "Conversion-optimized platform for healthcare financial services.",
      bg: "bg-gray-50",
      img: "/generated/image-healthcare-technology-interface-with-cle-1765565087075-5.webp",
      dark: false
    },
    {
      client: "CommerceRoad",
      desc: "Strategic website for an eCommerce borrowing platform.",
      bg: "bg-[#f8f8f8]",
      img: "/generated/image-modern-ecommerce-platform-interface-show-1765565089290-6.webp",
      dark: false,
      full: true
    },
    {
      client: "Movi Partners",
      desc: "Professional web system for a venture capital firm.",
      bg: "bg-gray-100",
      img: "/generated/image-venture-capital-office-with-modern-desig-1765565091510-7.webp",
      dark: false
    },
    {
      client: "Dante AI",
      desc: "Long-term partnership delivering ongoing website optimization and autonomy.",
      bg: "bg-[#0a0a0a]",
      img: "",
      dark: true
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We transform underperforming websites into conversion systems</span> that growth-stage tech companies can operate autonomously—no developer dependencies, no bottlenecks.
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
