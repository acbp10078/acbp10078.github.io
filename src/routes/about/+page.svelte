<script lang=ts>
    import {assets} from "$app/paths"
    let name = "Aaron Clark B. Perez";
    let title = "3rd Year College Student";
    let course = "Bachelor of Science in Information Technology";
    let location = "Olongapo City";
    let passions = ["Technology", "Coding", "Journalism", "Public Speaking", "Public Service"];
    let experience = 3;
    let projects = ["Simple Calculator", "Personal Portfolio", "Library Management System"];
    let activities = [
      "Journalism Training in Radio and TV Broadcasting at Olongapo City National High School",
      "Organization Management as Student Council President of CCS"
    ];
  
    let socialLinks = [
      { name: "Facebook", url: "https://www.facebook.com/aaronclark.perez/", icon: "fab fa-facebook-f" },
      { name: "Gmail", url: "mailto:aaronclarkperez@gmail.com", icon: "fas fa-envelope" },
      { name: "GitHub", url: "https://github.com/acbp10078", icon: "fab fa-github" },
    ];
  </script>
  
  <div class="max-w-4xl mx-auto p-6 bg-white bg-opacity-80 shadow-md rounded-lg my-8">
    <div class="flex flex-col md:flex-row items-center md:items-start">
      <img src="/assets/aaron.JPG" alt={name} class="w-40 h-40 rounded-full object-cover mb-6 md:mb-0 md:mr-8 shadow-md">
      <div class="flex-1">
        <h1 class="text-3xl font-bold text-gray-800 mb-2">{name}</h1>
        <p class="text-lg text-blue-600 mb-1">{title}</p>
        <p class="text-md text-gray-700 mb-3">{course}</p>
        <p class="text-md text-gray-600 mb-5">
          Based in {location}
        </p>
        <div class="mb-5">
          <h2 class="text-xl font-semibold text-gray-800 mb-2">About Me</h2>
          <p class="text-gray-600 leading-relaxed">
            As a passionate student pursuing a {course}, I'm deeply interested in {passions.join(', ')}. 
            With {experience} years of experience in my studies, I've developed a strong foundation in my field and 
            continue to expand my knowledge and skills.
          </p>
        </div>
        <div class="mb-5">
          <h2 class="text-xl font-semibold text-gray-800 mb-2">Projects</h2>
          <ul class="list-disc list-inside text-gray-600">
            {#each projects as project}
              <li>{project}</li>
            {/each}
          </ul>
        </div>
        <div class="mb-5">
          <h2 class="text-xl font-semibold text-gray-800 mb-2">Extracurricular Activities</h2>
          <ul class="list-disc list-inside text-gray-600">
            {#each activities as activity}
              <li>{activity}</li>
            {/each}
          </ul>
        </div>
        <div class="flex space-x-4">
          {#each socialLinks as link}
            <a href={link.url} class="text-blue-500 hover:text-blue-700 transition-colors duration-300" aria-label={link.name}>
              <i class="{link.icon} fa-lg" aria-hidden="true"></i>
            </a>
          {/each}
        </div>
      </div>
    </div>
  </div>
  
  <style>
    @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css');
  </style>