---
layout: page
title: Public engagement
permalink: /public-engagement/
published: true
---

<p class="engagement-intro">I share psychological science through hands-on activities, public talks, science festivals and creative events.</p>

<div class="outreach-montage" aria-label="Photographs from public engagement events">
  <a href="{{ '/images/public-engagement/science-outreach-classroom.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/science-outreach-classroom.jpg' | relative_url }}" alt="Demonstrating visual illusions with goggles and a spiral in a classroom." /></a>
  <a href="{{ '/images/public-engagement/research-talk.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/research-talk.jpg' | relative_url }}" alt="Giving a talk about language and perception." /></a>
  <a href="{{ '/images/public-engagement/mysteries-of-the-mind-banner.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/mysteries-of-the-mind-banner.jpg' | relative_url }}" alt="An outreach demonstrator beside the Mysteries of the Mind banner." /></a>
  <a href="{{ '/images/public-engagement/children-science-outreach.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/children-science-outreach.jpg' | relative_url }}" alt="Children and visitors trying activities at a psychology stall." loading="lazy" /></a>
  <a href="{{ '/images/public-engagement/public-engagement-campus.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/public-engagement-campus.jpg' | relative_url }}" alt="Visitors taking part in an outdoor public engagement event." loading="lazy" /></a>
  <a href="{{ '/images/public-engagement/mysteries-of-the-mind-stall.jpg' | relative_url }}"><img src="{{ '/images/public-engagement/mysteries-of-the-mind-stall.jpg' | relative_url }}" alt="Demonstrators at the Mysteries of the Mind and Psychology stand." loading="lazy" /></a>
</div>

## Pop-Up Psychology

I run **Pop-Up Psychology**, bringing short experiments and demonstrations about perception, memory, language and the brain to schools and public events. The activity guides are freely available for others to use.

{% assign activities = 'buzz-wire-task|Buzz Wire Task,hollow-face-illusion|Hollow Face Illusion,stroop-effect|Stroop Effect,rubber-hand-illusion|Rubber Hand Illusion,live-eeg-brain-signals|Live EEG Brain Signals,tower-of-hanoi|Tower of Hanoi,semantic-priming|Semantic Priming,upside-down-goggles|Upside-Down Goggles' | split: ',' %}
<div class="activity-montage" aria-label="Pop-Up Psychology activity guides">
{% for activity in activities %}
  {% assign card = activity | split: '|' %}
  <a href="{{ '/images/public-engagement/pop-up-psychology/' | append: card[0] | append: '.jpg' | relative_url }}" aria-label="View {{ card[1] }} activity guide"><img src="{{ '/images/public-engagement/pop-up-psychology/' | append: card[0] | append: '.jpg' | relative_url }}" alt="{{ card[1] }} activity guide" loading="lazy" /></a>
{% endfor %}
</div>

<p class="engagement-contact">If you’re a schoolteacher or organising an event and would like to arrange a visit, <a href="mailto:{{ site.email }}">get in touch</a>.</p>
