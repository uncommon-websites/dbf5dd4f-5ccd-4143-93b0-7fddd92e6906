<script lang="ts">
  const clients = [
    "American Bitcoin",
    "XFX",
    "Rare Origins",
    "Flychain",
    "CommerceRoad",
    "Movi Partners",
    "Dominion",
    "Dante AI"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#1a1a1a] via-[#2a2a2a] to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#0a0a0a_0%,#1a1a1a_30%,#f5f5f5_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      Transform your website into a conversion system. <span class="text-gray-400">Give your marketing team the autonomy to move fast—without waiting on developers.</span>
    </h1>
  </div>

  <div class="border-t border-gray-700 pt-8 flex flex-wrap gap-8 md:gap-12 items-center opacity-50">
    {#each clients.slice(0, 6) as client}
      <div class="h-8 flex items-center justify-center text-sm font-medium text-gray-500">{client}</div>
    {/each}
  </div>
</section>
