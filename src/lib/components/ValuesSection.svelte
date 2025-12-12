<script lang="ts">
  const photos = [
    {
      title: "Complete Training & Resources",
      desc: "60-minute post-launch workshop, lifetime resource library access, complete documentation, and 30 days of technical support.",
      img: "/generated/image-modern-tech-startup-office-with-clean-de-1765564925193-3.webp"
    },
    {
      title: "Component-Based Systems",
      desc: "Enterprise-level capability with consumer-level ease. Build new pages in hours, not weeks, using our proprietary framework.",
      img: "/generated/image-designer-working-on-component-based-webs-1765564927471-4.webp"
    },
    {
      title: "Strategic Partnership Options",
      desc: "Need ongoing support? Growth Partnership retainers start at $4,750/month with 3-month minimum for teams wanting continued strategic guidance.",
      img: "/generated/image-strategic-business-meeting-between-consu-1765564929737-5.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">Everything you need for marketing autonomy.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      We don't just build websites and disappear. Every sprint includes comprehensive training, resources, and support to ensure your team can operate independently and confidently from day one.
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
