<script>
  let projects = [
    {
      id: 1,
      image: "/images/projects/project_1.jpg",
      title: "Лендинг Художественной галереи",
      link: "https://artyaexe.github.io/blanchard/",
    },
    {
      id: 2,
      image: "/images/projects/project_2.jpg",
      title: "Сайт-визитка фотографа",
      link: "https://artyaexe.github.io/dinazzz-photo/",
    },
    {
      id: 3,
      image: "/images/projects/project_3.jpg",
      title: "Сайт Медицинского центра",
      link: "https://artyaexe.github.io/go-corona/",
    },
    {
      id: 4,
      image: "/images/projects/project_4.jpg",
      title: "Сайт-визитка Застройщика",
      link: "https://artyaexe.github.io/evklid/",
    },
    {
      id: 5,
      image: "/images/projects/project_5.jpg",
      title: "Лендинг VPN-приложения",
      link: "https://artyaexe.github.io/my-vpn/",
    },
    {
      id: 6,
      image: "/images/projects/project_6.jpg",
      title: "Лендинг Проката автомобилей",
      link: "https://artyaexe.github.io/cars-hw/",
    },
  ];
</script>

<section class="projects">
  <div class="container">
    <h2 class="projects-title" data-aos="fade-up">Мои проекты</h2>
    <ul class="projects-list">
      {#each projects as project (project.id)}
        <li class="projects-list__item" data-aos="fade-up">
          <a class="project-link" href={project.link} target="_blank">
            <div class="top-item">
              <img src={project.image} alt="" />
            </div>
            <div class="bottom-item">
              <p class="project-name">{project.title}</p>
            </div>
          </a>
        </li>
      {/each}
    </ul>
  </div>
</section>

<style>
  .projects {
    padding: 50px 0;
    background-color: var(--color-light);
  }

  .projects-title {
    text-align: center;
  }

  .projects-title {
    color: var(--color-dark);
    font-size: 40px;
    font-style: normal;
    line-height: 140%;
    margin-bottom: 20px;
    letter-spacing: -0.5px;
    font-weight: 700;
  }

  .projects-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
  }

  .projects-list__item {
    border-radius: 20px;
    box-shadow: 0px 5px 35px 0px rgba(0, 0, 0, 0.25);
  }

  .top-item {
    padding: 10px;
    background-color: var(--color-dark-light);
    border-radius: 20px;
    overflow: hidden;
    transition: all 0.7s ease;
  }

  .top-item img {
    transition: all 0.3s ease-in-out;
    border-radius: 15px;
    width: 320px;
    height: auto;
  }

  .bottom-item {
    text-align: center;
    padding: 20px;
  }

  .project-name {
    color: var(--color-dark);
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: 24px;
  }

  .project-link:focus {
    outline: none;
  }

  .project-link:focus .top-item {
    background-color: var(--color-beige-light);
  }

  .project-link:hover .top-item {
    background-color: var(--color-beige);
  }

  .project-link:active .top-item {
    background-color: var(--color-beige-light);
  }

  .project-link:active > .top-item > img {
    transform: scale(0.95);
  }
</style>
