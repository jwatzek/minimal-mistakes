---
title: "Code"
permalink: /code/
header:
  image: unsplash-code.jpeg
  caption: "Photo credit: [Ilya Pavlov](https://unsplash.com/@ilyapavlov)"
---

{% include toc title=page.title icon="code" %}

My languages of choice are R and Python for all things data science, but I find my way around Matlab and SAS as well. I use LaTeX for typesetting and the usual suspects for web development (HTML, CSS/Bootstrap, JavaScript, jQuery). 

Recently, I've been learning Java and XML for Android mobile development. My latest project is WhatsOb, an app for behavioral observations. My code's available on Github wherever possible (personal: [@jwatzek](http://github.com/jwatzek), organizational: [@gsu-lrc](http://github.com/gsu-lrc)).

**Note.** Most of my R data analysis scripts currently live in private repos until they're (ready to be) published alongside a manuscript.
{: .notice}

## Stimulus Presentation

I use Python 2.7 (with Pygame and SciPy) to run computer experiments with the monkeys, kids, and undergrads. 

<!-- arcade table + sketchup design -->

I learned and introduced Python to the Language Research Center as an open-source, cross-platform, readable language to write experiments. I wrote a toolbox module specific to this research center and also run workshops focused on hands-on coding. As a result, our research coordinators and most graduate students (all with no prior programming experience) now have a working knowledge of computational concepts in general and Python in specific, enabling them to adapt, fix, and write their own programmes.

You can find the code for all of my programmes and those I've contributed to on the Github page I maintain for the Language Research Center [@gsu-lrc](http://github.com/gsu-lrc). 

{% capture fig_img %}
[![Python]({{ site.url }}/images/xkcd_python.png)](https://xkcd.com/353/)
{% endcapture %}

{% capture fig_caption %}
"I wrote 20 short programs in Python yesterday.  It was wonderful. Perl, I'm leaving you." --*xkcd*
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>{{ fig_caption | markdownify | remove: "<p>" | remove: "</p>" }}</figcaption>
</figure>

## App Development

**WhatsOb: An Android app for note-taking during behavioral observations**

For behavioral observations of both humans and animals, it is crucial not to lose focus of the subjects at hand, and yet take detailed, accurate, and timely notes. Mobile devices are highly versatile, unobtrusive, and portable tools that lend themselves to the task. While there are numerous note-taking apps, they typically have several shortcomings for use as scientific tools: 

1. Typing on a touchscreen keyboard is tedious, takes time, and is prone to typos.
2. Dates and times have to be recorded manually.
3. The raw data typically require extensive reformatting prior to data analysis. 

To address these problems, I developed WhatsOb, an Android app designed to allow for fast but accurate data capture with minimal device interaction. Preconfigured quick text buttons replace tedious typing and researchers can set up flexible observation formats for different study populations. The app allows configuration of several sets of quick text buttons to minimize screen clutter and increase versatility. Additionally, all entries are time-stamped automatically and researchers can schedule timers in the form of sound or onscreen notifications. Data files are exported as plain text or comma-separated values (CSV) files via email and common cloud file hosting services. 

Actual use cases in my lab are three types of behavioral observations: scan samples, focal samples, and ad lib data collection.


## Website Development

{% capture fig_ll %}
[![Living Links website]({{ site.url }}/images/living_links.png){: .align-center}](http://emory.edu/LIVING_LINKS)
{% endcapture %}

{% capture fig_mojo %}
[![Mojo Fitness website]({{ site.url }}/images/mojo_fitness.png){: .align-center}](http://www.mojo.fitness)
{% endcapture %}

{% capture fig_pca %}
[![Peach Cobbler ATL website]({{ site.url }}/images/peachcobbler.png){: .align-center}](http://www.peachcobbleratl.com)
{% endcapture %}

I made the website for my previous lab at the [Living Links Center for the Advanced Study of Ape and Human Evolution](http://emory.edu/LIVING_LINKS). It's simple and straightforward HTML and CSS from a time before responsive design was much of a thing.

As an avid rock climber, I'm part of a climbing shoe resole shop called [Peach Cobbler ATL](http://www.peachcobbleratl.com) and also have a friend who started a business as a personal trainer and who needed a [logo and a website](http://www.mojo.fitness/). Both websites are heavily bootstrapped with a few JS and PHP elements here and there.

And I built the website you're on right now with [Jekyll](http://jekyllrb.com/) and  the [Minimal Mistakes Theme](https://mmistakes.github.io/minimal-mistakes/). You can find the code [here](http://github.com/jwatzek/jwatzek.github.io).

<figure class="third">
    {{ fig_ll | markdownify | remove: "<p>" | remove: "</p>" }}
    {{ fig_mojo | markdownify | remove: "<p>" | remove: "</p>" }}
    {{ fig_pca | markdownify | remove: "<p>" | remove: "</p>" }}
    <figcaption>Landing pages of Living Links, Mojo Climbing & Fitness, and Peach Cobbler ATL.</figcaption>
</figure>


