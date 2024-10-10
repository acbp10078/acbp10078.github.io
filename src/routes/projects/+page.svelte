<script>
    // Sample project data - replace with your actual projects
    let projects = [
      {
        title: "Project 1",
        description: "This project is the 1st project that I've done using the simplest HTML and CSS with the guidance of Sir Joseph Angelo Pusing. Despite that, the history behind this is difficult since I was the only one giving effort to do the project",
        image: "/assets/1proj.jpg", // Replace with your actual image path
        link: "#" // Replace with actual project link if available
      },
      {
        title: "Project 2",
        description: "This is one of the good projects that I've done with the guidance of my friends but at the same time wasn't able to finish on time due to the fact that my laptop was still a cheap old laptop.",
        image: "/assets/LMS.jpg", // Replace with your actual image path
        link: "#" // Replace with actual project link if available
      }
    ];
  </script>
  
  <div class="max-w-6xl mx-auto p-6">
    <h1 class="text-3xl font-bold text-center mb-10">My Projects</h1>
    
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      {#each projects as project}
        <div class="bg-white rounded-lg shadow-md overflow-hidden">
          <img src={project.image} alt={project.title} class="w-full h-64 object-cover">
          <div class="p-6">
            <h2 class="text-2xl font-semibold mb-2">{project.title}</h2>
            <p class="text-gray-600 mb-4">{project.description}</p>
            <a href={project.link} class="inline-block bg-blue-500 text-white py-2 px-4 rounded hover:bg-blue-600 transition-colors duration-300">
              View Project
            </a>
          </div>
        </div>
      {/each}
    </div>
  </div>