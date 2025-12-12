<script lang="ts">
  const photos = [
    {
      title: "Automotive Excellence",
      desc: "Our onsite tech support team brings hands-on expertise to automotive dealerships, ensuring systems run smoothly.",
      img: "https://images.unsplash.com/photo-1619642751034-765dfdf7c58e?auto=format&fit=crop&q=80&w=400"
    },
    {
      title: "Cross-Functional Teams",
      desc: "Our project managers bridge technology and marketing, delivering integrated solutions that drive business results.",
      img: "https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=800"
    },
    {
      title: "Creative Innovation",
      desc: "Our digital marketing team brings fresh perspectives to technology projects, creating solutions that resonate with users.",
      img: "https://images.unsplash.com/photo-1557804506-669a67965ba0?auto=format&fit=crop&q=80&w=400"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We're building a team that solves real problems.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      From automotive tech support to project management and digital marketing, we're growing our capabilities to better serve mid-market companies. Our culture values expertise, collaboration, and the drive to turn business challenges into technical solutions.
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
