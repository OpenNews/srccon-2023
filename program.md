---
section: program
permalink: /program/
title: Our Program
---

# Our Program

The following sessions have been confirmed so far for {{ page.event_name }}. Thank you to everyone who submitted proposals! We still have a handful of sessions left to finalize, and descriptions here will evolve in the weeks leading up to {{ page.event_name }}.

We'll publish the complete schedule with session dates and times soon.

## Sessions 

Thank you to the [community panel](#community-review) that helped us during our review process! Our conference schedule this year will include the sessions below.

<div class="session-proposal-list">{% comment %}The one-line if statement below is ugly but prevents massive whitespace in the template{% endcomment %}
{% for proposal in site.data.sessions %}
    <div class="session-proposal" id="proposal-{{ proposal.id }}">
        <h4 class="session-title"><a href="#proposal-{{ proposal.id }}">{{ proposal.title }}</a></h4>
        {% if proposal.facilitators %}<p class="facilitator">Facilitated by {{ proposal.facilitators }}</p>{% endif %}
        <p class="session-description">{{ proposal.description | markdownify }}</p>
    </div>
{% endfor %}
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script src="/media/js/listfilter.min.js"></script>
<script>
var filter = ListFilter({
    listContainer: '.session-proposal-list',
    filterItemClass: '.session-proposal'
});
</script>

<span id="community-review"></span>

## Community reviewers

We'd also like to thank the folks who helped us select this amazing slate of sessions! Each year's program review includes a panel of community members with a range of experiences and perspectives to make sure SRCCON has sessions that respond to your needs.

Thank you, community reviewers!

* Amethyst Davis
* Andrew Calderon
* Danielle Alberti
* Kae Petrin
* Melissa Fronczek
* Yoohyun Jung
