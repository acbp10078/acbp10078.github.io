<script>

    export let tabs = [
        { name: "Projects ", link: "/projects" },
        { name: "About me", link: "/about" }, 
    ];
</script>

<header
    class="z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid py-4 bg-slate-950 border-violet-950 bg-transparent border-transparent"
>
<a href="/" class="text-decoration-none">
    <h1 class="font-medium">
      <b class="font-bold poppins">Aaron Clark Perez</b>
    </h1>
  </a>

    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}
            <a
                href={tab.link}
                class="duration-200 hover:text-violet-400"
                target={index === 2 ? "_blank" : ""}
            >
                <p>{tab.name}</p>
            </a>
        {/each}


    </div>
</header>