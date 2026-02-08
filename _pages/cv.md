---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div style="max-width:900px; margin:auto; line-height:1.5; font-size:17px;">

<!-- Education -->
<h2 style="border-bottom:1px solid #000;">Education</h2>

<ul>
  <li><strong>B.Tech in Electrical Engineering</strong>, GITAM University — 2027 (expected)</li>
  <li><strong>Diploma</strong>, Government Polytechnic, Visakhapatnam — 2024</li>
</ul>

<!-- Work Experience -->
<h2 style="border-bottom:1px solid #000;">Work Experience</h2>

<p><strong>Summer 2025 — Indian Institute</strong></p>
<ul>
  <li>GitHub University</li>
  <li>Duties: Updates and improvements to template</li>
  <li>Supervisor: The Users</li>
</ul>

<p><strong>Fall 2015 — Research Assistant</strong></p>
<ul>
  <li>GitHub University</li>
  <li>Duties: Merging pull requests</li>
  <li>Supervisor: Professor Hub</li>
</ul>

<p><strong>Summer 2015 — Research Assistant</strong></p>
<ul>
  <li>GitHub University</li>
  <li>Duties: Tagging issues</li>
  <li>Supervisor: Professor Git</li>
</ul>

<!-- Skills -->
<h2 style="border-bottom:1px solid #000;">Skills</h2>

<ul>
  <li>Skill 1</li>
  <li>Skill 2
    <ul>
      <li>Sub-skill 2.1</li>
      <li>Sub-skill 2.2</li>
      <li>Sub-skill 2.3</li>
    </ul>
  </li>
  <li>Skill 3</li>
</ul>

<!-- Publications -->
<h2 style="border-bottom:1px solid #000;">Publications</h2>

<ul>
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

<!-- Talks -->
<h2 style="border-bottom:1px solid #000;">Talks</h2>

<ul>
{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

<!-- Teaching -->
<h2 style="border-bottom:1px solid #000;">Teaching</h2>

<ul>
{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

<!-- Service -->
<h2 style="border-bottom:1px solid #000;">Service and Leadership</h2>

<ul>
  <li>Currently signed in to 43 different Slack teams</li>
</ul>

</div>
