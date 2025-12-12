<script lang="ts">
  const stats = [
    {
      label: "2-4 Week Sprints",
      desc: "Most growth-stage tech companies complete their Growth Engine Sprint in 2-4 weeks. We move fast with a strategic workshop, design system, complete Webflow build, and team training—all within a month. Your timeline flexes based on feedback turnaround, but we're ready when you are.",
      img: "/generated/image-calendar-with-sprint-timeline-marked-cle-1765565075416-0.webp"
    },
    {
      label: "$15k-$25k Range",
      desc: "Growth Engine Sprints start at $15k, with most growth-stage tech companies falling in the $15k-$25k range. You get strategic workshop, 5 core pages, complete Webflow build with marketing autonomy framework, training, and lifetime resource access. Month-to-month retainers also available starting at $4,750.",
      img: "/generated/image-professional-handshake-or-contract-signi-1765565077757-1.webp"
    },
    {
      label: "2-3x to 12x+ Conversions",
      desc: "Our conversion framework is built on user psychology principles tested across hundreds of B2B websites. While results vary by baseline, clients report conversion improvements ranging from 2-3x to 12x+ depending on their starting point. We focus on measurable outcomes, not vanity metrics.",
      img: "/generated/image-upward-trending-graph-or-chart-showing-g-1765565080219-2.webp"
    },
    {
      label: "1-2 Week Autonomy",
      desc: "Your marketing team operates independently within 1-2 weeks after launch. Our proprietary framework makes Webflow accessible to non-technical marketers with component-based systems and CMS structures. No more waiting weeks for simple changes—your team moves at the speed of your business.",
      img: "/generated/image-marketing-professional-confidently-worki-1765565082476-3.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Real numbers from real clients. Here's what you can expect when working with Nube.
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
