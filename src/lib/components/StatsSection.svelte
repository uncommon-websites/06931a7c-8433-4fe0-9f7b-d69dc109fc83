<script lang="ts">
  const stats = [
    {
      label: "Fortune 500 Trust",
      desc: "We've earned the trust of major enterprise clients including EY, Deloitte, IBM, AT&T, Boeing, Airbus, Delta Air Lines, and Eli Lilly. Our track record with Fortune 500 companies demonstrates our ability to deliver enterprise-grade solutions while maintaining the personal touch of a dedicated partner.",
      img: "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Microsoft Certified",
      desc: "As certified Microsoft Partners, we bring deep expertise in Microsoft technologies and enterprise solutions. This partnership enables us to provide best-in-class infrastructure services, from network security to cloud solutions, backed by Microsoft's industry-leading platforms.",
      img: "https://images.unsplash.com/photo-1633356122544-f134324a6cee?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Multi-Industry Expertise",
      desc: "From automotive dealerships to healthcare systems, manufacturing to hospitality, we've successfully delivered solutions across diverse industries. Our experience spans consulting, technology, aviation, telecommunications, real estate, and more—giving us unique insights into varied business challenges.",
      img: "https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Growing Team",
      desc: "We're actively expanding our capabilities with new positions in automotive tech support, project management, and digital marketing. Our growth reflects our commitment to providing comprehensive technology and consulting services to mid-market companies who need reliable partners.",
      img: "https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&q=80&w=200"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Discover what sets Knowtion apart—our client relationships, certifications, and the expertise that drives results.
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
