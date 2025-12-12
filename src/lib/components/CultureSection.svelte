<script lang="ts">
  const cards = [
    {
      title: "Marketing Teams Shouldn't Wait...",
      subtitle: "They Should Move Fast.",
      image: "/generated/image-marketing-team-collaborating-around-a-la-1765564917480-0.webp"
    },
    {
      title: "Websites Shouldn't Be Bottlenecks...",
      subtitle: "They Should Be Growth Assets.",
      image: "/generated/image-close-up-of-a-laptop-screen-showing-webs-1765564920642-1.webp"
    },
    {
      title: "You Don't Need More Developers...",
      subtitle: "You Need Marketing Autonomy.",
      image: "/generated/image-confident-marketing-professional-working-1765564922953-2.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      We give marketing teams their time back. No more waiting weeks for simple changes. No more developer dependencies. Just a website system you can operate autonomously.
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
