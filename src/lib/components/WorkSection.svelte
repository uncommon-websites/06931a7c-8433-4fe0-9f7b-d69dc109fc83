<script lang="ts">
  const projects = [
    {
      client: "Ken Ganley Auto Group",
      desc: "Comprehensive IT infrastructure and dealership technology solutions.",
      bg: "bg-gray-900",
      img: "https://images.unsplash.com/photo-1562911791-c7a97b729ec5?auto=format&fit=crop&q=80&w=800",
      dark: true
    },
    {
      client: "Lake Health",
      desc: "Healthcare IT systems and network security implementation.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1519494026892-80bbd2d6fd0d?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "Conrex Property Management",
      desc: "Custom property management software and business process optimization.",
      bg: "bg-gray-200",
      img: "https://images.unsplash.com/photo-1560518883-ce09059eeffa?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "PureCars",
      desc: "Mobile and web application development for automotive industry.",
      bg: "bg-black",
      img: "",
      dark: true
    },
    {
      client: "Chick-fil-A",
      desc: "Enterprise technology consulting and system integration.",
      bg: "bg-gray-50",
      img: "https://images.unsplash.com/photo-1567521464027-f127ff144326?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true
    },
    {
      client: "Malish Corporation",
      desc: "EOS framework implementation and Lean Six-Sigma consulting.",
      bg: "bg-gray-200",
      img: "https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "PERQ",
      desc: "Full-stack development and cloud infrastructure management.",
      bg: "bg-gray-100",
      img: "https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=800",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We integrate software development, strategic consulting, and IT infrastructure</span> to deliver reliable technology solutions that drive business growth and operational excellence.
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
