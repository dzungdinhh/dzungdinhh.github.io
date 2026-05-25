---
layout: homepage
---

<div class="intro-section">
  <h1 class="intro-name">{{ site.title }}</h1>

  <div class="intro-copy">
    <p>I am a Ph.D. student in Computer Science at UNC-Chapel Hill, working closely with <a href="https://scholar.google.com/citations?user=CqH_t6MAAAAJ&hl=en">Prof. Junier Oliva</a> in the <a href="https://sites.google.com/cs.unc.edu/lupalab/projects">LUPA Lab</a>. For Summer 2026, I am also joining <a href="https://www.hitachi.com/en-us/">Hitachi America, Ltd.</a>'s Financial Innovation Lab as a Research Intern. My research focuses on machine learning methods for reliable prediction and efficient information acquisition, with applications in active feature acquisition, longitudinal data, and trustworthy ML for scientific discovery.</p>

    <p>I received my B.S. in Computer Science with a minor in Mathematics from Dickinson College, where I worked with <a href="https://www.dickinson.edu/johnmaccormick">Prof. John MacCormick</a> on object detection and computer graphics projects. Previously, I was an intern at the <a href="https://csl.illinois.edu/">UIUC Coordinated Science Laboratory</a> and a community researcher at <a href="https://cohere.com/research">Cohere For AI</a>.</p>
  </div>

  <figure class="intro-photo">
    <img src="{{ site.avatar }}" alt="{{ site.title }} profile photo">
    <figcaption class="profile-card">
      {% if site.email %}
      <div class="profile-email">{{ site.email }}</div>
      {% endif %}
      <div class="profile-links" aria-label="Profile links">
        {% if site.google_scholar %}
        <a href="{{ site.google_scholar }}" aria-label="Google Scholar">
          <i class="ai ai-google-scholar"></i>
        </a>
        {% endif %}
        {% if site.linkedin %}
        <a href="{{ site.linkedin }}" aria-label="LinkedIn">
          <i class="fab fa-linkedin"></i>
        </a>
        {% endif %}
      </div>
    </figcaption>
  </figure>
</div>

## Education
- 2024-Present: Ph.D. in Computer Science, [The University of North Carolina at Chapel Hill](https://www.unc.edu/)
- 2024-2026: M.S. in Computer Science, en route to Ph.D., [The University of North Carolina at Chapel Hill](https://www.unc.edu/)
- 2020-2024: B.S. in Computer Science, [Dickinson College](https://www.dickinson.edu/)

<!-- ## Research Interests

- **Computer Vision:** image recognition, image generation, video captioning
- **Machine Learning:** meta-learning, incremental learning, transfer learning -->

<!-- ## News

- **[Feb. 2020]** Our paper about incremental learning is accepted to CVPR 2020.
- **[Feb. 2020]** We will host the ACM Multimedia Asia 2020 conference in Singapore!
- **[Sept. 2019]** Our paper about few-shot learning is accepted to NeurIPS 2019.
- **[Mar. 2019]** Our paper about few-shot learning is accepted to CVPR 2019. -->


{% include_relative _includes/publications.md %}

<p class="last-updated">Last updated: May 2026</p>

<!-- {% include_relative _includes/services.md %} -->
