---
layout: default
title: Shane Lindsay
published: true
---

<section class="hero">
  <div class="container hero-grid">
    <div class="hero-copy">
      <p class="eyebrow">Psychology lecturer · University of Hull</p>
      <h1>Language, cognition, and the brain.</h1>
      <p class="lede">
        I study how language interacts with perception, action, and memory, drawing on
        behavioural methods, eye tracking, and cognitive neuroscience. I run the CogLang lab.
      </p>
      <div class="hero-actions">
        <a class="button" href="{{ '/research/' | relative_url }}">Research</a>
        <a class="button ghost" href="{{ '/teaching-and-learning/' | relative_url }}">Teaching</a>
      </div>
      <div class="hero-links">
        <a href="https://www.hull.ac.uk/faculties/staff-profiles/shane-lindsay">University profile</a>
        <a href="https://hull-repository.worktribe.com/person/315748/shane-lindsay/outputs">Worktribe outputs</a>
      </div>
    </div>
    <div class="hero-card">
      <img src="{{ '/images/me.jpg' | relative_url }}" alt="Photo of Shane Lindsay" />
      <div class="hero-card-meta">
        <p class="hero-name">Shane Lindsay</p>
        <p class="hero-role">Lecturer in Psychology</p>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-heading">
      <h2>Research focus</h2>
      <p>Core themes in my work, spanning language, memory, and the visual world.</p>
    </div>
    <div class="grid grid-3">
      <div class="card">
        <span class="tag">Word learning</span>
        <h3>Sleep, memory, and consolidation</h3>
        <p>How new words are acquired, stabilised, and integrated over time.</p>
      </div>
      <div class="card">
        <span class="tag">Speech &amp; action</span>
        <h3>Perception and production</h3>
        <p>How perceptual and motor systems interact during spoken-language processing.</p>
      </div>
      <div class="card">
        <span class="tag">Vision &amp; language</span>
        <h3>Event representation</h3>
        <p>How visual and linguistic cues combine to build dynamic mental models.</p>
      </div>
    </div>
  </div>
</section>

<section class="section alt">
  <div class="container">
    <div class="section-heading">
      <h2>Teaching &amp; supervision</h2>
      <p>Research methods, statistics, and applied psychology across undergraduate and postgraduate teaching.</p>
    </div>
    <div class="grid grid-2">
      <div class="card">
        <h3>Research methods leadership</h3>
        <p>Module leadership and curriculum design for research methods and statistics in psychology.</p>
      </div>
      <div class="card">
        <h3>Project supervision</h3>
        <p>Supervision for undergraduate dissertations, MSc/MRes projects, and doctoral research.</p>
      </div>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-heading">
      <h2>CogLang lab</h2>
      <p>A collaborative lab investigating cognition and language with behavioural and neuroscience tools.</p>
    </div>
    <div class="grid grid-2">
      <div class="card">
        <h3>Methods</h3>
        <p>Behavioural experiments, eye tracking, EEG, TMS, and related cognitive neuroscience techniques.</p>
      </div>
      <div class="card">
        <h3>Opportunities</h3>
        <p>Opportunities for undergraduate assistants, Masters students, and PhD applicants.</p>
      </div>
    </div>
  </div>
</section>

<section class="section alt">
  <div class="container">
    <div class="section-heading">
      <h2>Latest writing</h2>
      <p>Selected posts from the blog.</p>
    </div>
    <div class="posts">
      {% assign latest_posts = site.posts | slice: 0, 2 %}
      {% if latest_posts.size > 0 %}
        {% for post in latest_posts %}
          <article class="post-card">
            <div class="date">{{ post.date | date: "%B %e, %Y" }}</div>
            <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
            <a href="{{ post.url | relative_url }}" class="post-nav-link">Read the post</a>
          </article>
        {% endfor %}
      {% else %}
        <div class="card">
          <p>No posts yet. Check back soon for updates.</p>
        </div>
      {% endif %}
    </div>
  </div>
</section>
