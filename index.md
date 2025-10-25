---
layout: bio
---

I am a fifth-year PhD candidate in the [Human-Computer Interaction Institute](https://www.hcii.cmu.edu/) at Carnegie Mellon University, where I am very grateful to be co-advised by [Prof. Ken Holstein](https://kenholstein.com/) and [Prof. Haiyi Zhu](https://haiyizhu.com/).

My research focuses on transforming the current top-down and centralized approach to AI development, towards more community-driven, deliberative, and democratic processes. To achieve this vision, I develop systems and processes that empower communities impacted by AI to collaboratively shape its design, evaluation, and governance. My research has received Best Paper and Honorable Mention Awards at top HCI conferences, including CHI and UIST. I have also been recognized with the [K&L Gates Presidential Fellowship in Ethics and Computational Technologies](https://www.cmu.edu/ethics-ai/news/2025-fellows.html), [CASMI PhD Fellowship](https://casmi.northwestern.edu/), [Taiwanese GSSA Fellowship](https://www.scholarship.moe.gov.tw/), and as an [MLCommons ML and Systems Rising Star](https://mlcommons.org/about-us/programs/).

Previously, I hold an M.S. from Stanford University, where I worked with [Prof. James Landay](https://www.landay.org/) and [Prof. Elizabeth Murnane](https://engineering.dartmouth.edu/community/faculty/elizabeth-murnane) in the [Stanford HCI Group](https://hci.stanford.edu/). I also graduated summa cum laude in Electrical Engineering from [National Taiwan University](https://www.ntu.edu.tw/english/), as a [Phi Tau Phi Scholar](http://www.phitauphi.org.tw) and [Irving T. Ho Fellow](https://irvingthofoundation.github.io/ho-fellows.htm).

Research interests: human-computer interaction, social computing, participatory design, responsible AI

[&nbsp;tzushenk@cs.cmu.edu&nbsp;] [&nbsp;[curriculum vitae](/assets/TzuShengKuo_CV.pdf)&nbsp;] [&nbsp;[google&nbsp;scholar](https://scholar.google.com/citations?user=i305250AAAAJ&hl=en)&nbsp;] [&nbsp;[twitter](https://twitter.com/tzushengkuo)&nbsp;] [&nbsp;[bluesky](https://bsky.app/profile/tskuo.bsky.social)&nbsp;] [&nbsp;[linkedin](https://www.linkedin.com/in/tzu-sheng-kuo)&nbsp;]

<div class="project-list-highlight">

  <h2>Main research: community-driven AI design, evaluation, and governance</h2>

  <h3>lead author papers</h3>

  <div class="project-list">
    <ul>
      {% for project in site.projects reversed %}

      {% capture project_year %}{{project.date | date: "%Y"}}{% endcapture %}
      {% capture project_published %}{{project.published}}{% endcapture %}
      {% capture project_category %}{{project.category}}{% endcapture %}
      {% capture project_subcategory %}{{project.subcategory}}{% endcapture %}

      {% if project_category == 'featured' and project_subcategory == 'first-author' and project_published != 'false' %}
        <li>

            <div class="project-col-wrapper">
                <div class="project-col project-col-1">
                    {% if project.paper %}
                    <a href="{{ project.paper }}" title="read PDF...">
                    {% endif %}
                    <img src="{{ project.thumbnail }}" alt="{{ project.title }}"/>
                    {% if project.paper %}
                    </a>
                    {% endif %}
                </div>
                <div class="project-col project-col-2">
                    <span class="project-title">{{ project.title }}</span>
                    {% if project.description %}
                    <div class="project-description">{{ project.description }}</div>
                    {% endif %}
                    {% if project.author %}
                    <div class="project-author">{{ project.author }}</div>
                    {% endif %}
                    {% if project.publication %}
                    <div class="project-publication">{{ project.publication }}</div>
                    {% endif %}
                    {% if project.award %}
                    <div class="project-award"><b>{{ project.award }}</b></div>
                    {% endif %}
                    <div class="project-link">
                    {% if project.paper %}
                    <a href="{{ project.paper }}">[paper]</a>
                    {% endif %}
                    {% if project.doi %}
                    <a href="{{ project.doi }}">[doi]</a>
                    {% endif %}
                    {% if project.arxiv %}
                    <a href="{{ project.arxiv }}">[arxiv]</a>
                    {% endif %}
                    {% if project.video %}
                    <a href="{{ project.video }}">[video]</a>
                    {% endif %}
                    {% if project.website %}
                    <a href="{{ project.website }}">[website]</a>
                    {% endif %}
                    {% if project.info %}
                    <a href="{{ project.url | prepend: site.baseurl }}">[more info]</a>
                    {% endif %}
                    </div>
                </div>
            </div>

        </li>
      {% endif %}
      {% endfor %}
    </ul>

  </div>

  <!-- <h3>collaborated papers</h3>

  <div class="project-list">
    <ul>
      {% for project in site.projects reversed %}

      {% capture project_year %}{{project.date | date: "%Y"}}{% endcapture %}
      {% capture project_published %}{{project.published}}{% endcapture %}
      {% capture project_category %}{{project.category}}{% endcapture %}
      {% capture project_subcategory %}{{project.subcategory}}{% endcapture %}

      {% if project_category == 'featured' and project_subcategory != 'first-author' and project_published != 'false' %}
        <li>

            <div class="project-col-wrapper">
                <div class="project-col project-col-1">
                    {% if project.paper %}
                    <a href="{{ project.paper }}" title="read PDF...">
                    {% endif %} 
                    <img src="{{ project.thumbnail }}" alt="{{ project.title }}"/>
                    {% if project.paper %}
                    </a>
                    {% endif %} 
                </div>
                <div class="project-col project-col-2">
                    <span class="project-title">{{ project.title }}</span>
                    {% if project.description %}
                    <div class="project-description">{{ project.description }}</div>
                    {% endif %}
                    {% if project.author %}
                    <div class="project-author">{{ project.author }}</div>
                    {% endif %}
                    {% if project.publication %}
                    <div class="project-publication">{{ project.publication }}</div>
                    {% endif %}
                    {% if project.award %}
                    <div class="project-award"><b>{{ project.award }}</b></div>
                    {% endif %}
                    <div class="project-link">
                    {% if project.paper %}
                    <a href="{{ project.paper }}">[paper]</a>
                    {% endif %}
                    {% if project.doi %}
                    <a href="{{ project.doi }}">[doi]</a>
                    {% endif %}
                    {% if project.video %}
                    <a href="{{ project.video }}">[video]</a>
                    {% endif %}
                    {% if project.permalink %}
                    <a href="{{ project.url | prepend: site.baseurl }}">[more info]</a>
                    {% endif %}
                    </div>
                </div>
            </div>

        </li>
      {% endif %}
      {% endfor %}
    </ul>
  </div> -->

</div>

## more research

<div class="project-list">
  <ul>
    {% for project in site.projects reversed %}

    {% capture project_year %}{{project.date | date: "%Y"}}{% endcapture %}
    {% capture project_published %}{{project.published}}{% endcapture %}
    {% capture project_category %}{{project.category}}{% endcapture %}
    {% capture project_subcategory %}{{project.subcategory}}{% endcapture %}

    {% if project_published != 'false' %}
    {% if project_category == 'research' %}
    {% if project_subcategory == 'more' %}
      <li>
          <div class="project-col-wrapper">
              <div class="project-col project-col-1">
                  {% if project.paper %}
                  <a href="{{ project.paper }}" title="read PDF...">
                  {% endif %}
                  <img src="{{ project.thumbnail }}" alt="{{ project.title }}"/>
                  {% if project.paper %}
                  </a>
                  {% endif %}
              </div>
              <div class="project-col project-col-2">
                  <span class="project-title">{{ project.title }}</span>
                  {% if project.description %}
                  <div class="project-description">{{ project.description }}</div>
                  {% endif %}
                  {% if project.author %}
                  <div class="project-author">{{ project.author }}</div>
                  {% endif %}
                  {% if project.publication %}
                  <div class="project-publication">{{ project.publication }}</div>
                  {% endif %}

                  {% if project.award %}
                  <div class="project-award"><b>{{ project.award }}</b></div>
                  {% endif %}

                  <div class="project-link">
                  {% if project.paper %}
                  <a href="{{ project.paper }}">[paper]</a>
                  {% endif %}
                  {% if project.doi %}
                  <a href="{{ project.doi }}">[doi]</a>
                  {% endif %}
                  {% if project.arxiv %}
                  <a href="{{ project.arxiv }}">[arxiv]</a>
                  {% endif %}
                  {% if project.video %}
                  <a href="{{ project.video }}">[video]</a>
                  {% endif %}
                  {% if project.website %}
                  <a href="{{ project.website }}">[website]</a>
                  {% endif %}
                  {% if project.info %}
                  <a href="{{ project.url | prepend: site.baseurl }}">[more info]</a>
                  {% endif %}
                  </div>

              </div>
          </div>
      </li>
    {% endif %}
    {% endif %}
    {% endif %}
    {% endfor %}

  </ul>
</div>

## organized workshops

<div class="project-list">
  <ul>
    {% for project in site.projects reversed %}

    {% capture project_year %}{{project.date | date: "%Y"}}{% endcapture %}
    {% capture project_published %}{{project.published}}{% endcapture %}
    {% capture project_category %}{{project.category}}{% endcapture %}
    {% capture project_subcategory %}{{project.subcategory}}{% endcapture %}

    {% if project_published != 'false' %}
    {% if project_category == 'workshop' %}
      <li>
          <div class="project-col-wrapper">
              <div class="project-col project-col-1">
                  {% if project.paper %}
                  <a href="{{ project.paper }}" title="read PDF...">
                  {% endif %}
                  <img src="{{ project.thumbnail }}" alt="{{ project.title }}"/>
                  {% if project.paper %}
                  </a>
                  {% endif %}
              </div>
              <div class="project-col project-col-2">
                  <span class="project-title">{{ project.title }}</span>
                  {% if project.description %}
                  <div class="project-description">{{ project.description }}</div>
                  {% endif %}
                  {% if project.author %}
                  <div class="project-author">{{ project.author }}</div>
                  {% endif %}
                  {% if project.publication %}
                  <div class="project-publication">{{ project.publication }}</div>
                  {% endif %}

                  {% if project.award %}
                  <div class="project-award"><b>{{ project.award }}</b></div>
                  {% endif %}

                  <div class="project-link">
                  {% if project.paper %}
                  <a href="{{ project.paper }}">[paper]</a>
                  {% endif %}
                  {% if project.doi %}
                  <a href="{{ project.doi }}">[doi]</a>
                  {% endif %}
                  {% if project.arxiv %}
                  <a href="{{ project.arxiv }}">[arxiv]</a>
                  {% endif %}
                  {% if project.video %}
                  <a href="{{ project.video }}">[video]</a>
                  {% endif %}
                  {% if project.website %}
                  <a href="{{ project.website }}">[website]</a>
                  {% endif %}
                  {% if project.info %}
                  <a href="{{ project.url | prepend: site.baseurl }}">[more info]</a>
                  {% endif %}
                  </div>

              </div>
          </div>
      </li>
    {% endif %}
    {% endif %}
    {% endfor %}

  </ul>
</div>

## other leadership

<div class="project-list">
  <ul>
    {% for project in site.projects reversed %}

    {% capture project_year %}{{project.date | date: "%Y"}}{% endcapture %}
    {% capture project_published %}{{project.published}}{% endcapture %}
    {% capture project_category %}{{project.category}}{% endcapture %}
    {% capture project_subcategory %}{{project.subcategory}}{% endcapture %}

    {% if project_published != 'false' %}
    {% if project_category == 'initiative' %}
      <li>
          <div class="project-col-wrapper">
              <div class="project-col project-col-1">
                  {% if project.paper %}
                  <a href="{{ project.paper }}" title="read PDF...">
                  {% endif %}
                  <img src="{{ project.thumbnail }}" alt="{{ project.title }}"/>
                  {% if project.paper %}
                  </a>
                  {% endif %}
              </div>
              <div class="project-col project-col-2">
                  <span class="project-title">{{ project.title }}</span>
                  {% if project.description %}
                  <div class="project-description">{{ project.description }}</div>
                  {% endif %}
                  {% if project.author %}
                  <div class="project-author">{{ project.author }}</div>
                  {% endif %}
                  {% if project.publication %}
                  <div class="project-publication">{{ project.publication }}</div>
                  {% endif %}

                  {% if project.award %}
                  <div class="project-award"><b>{{ project.award }}</b></div>
                  {% endif %}

                  <div class="project-link">
                  {% if project.paper %}
                  <a href="{{ project.paper }}">[paper]</a>
                  {% endif %}
                  {% if project.doi %}
                  <a href="{{ project.doi }}">[doi]</a>
                  {% endif %}
                  {% if project.arxiv %}
                  <a href="{{ project.arxiv }}">[arxiv]</a>
                  {% endif %}
                  {% if project.video %}
                  <a href="{{ project.video }}">[video]</a>
                  {% endif %}
                  {% if project.website %}
                  <a href="{{ project.website }}">[website]</a>
                  {% endif %}
                  {% if project.info %}
                  <a href="{{ project.url | prepend: site.baseurl }}">[more info]</a>
                  {% endif %}
                  </div>

              </div>
          </div>
      </li>
    {% endif %}
    {% endif %}
    {% endfor %}

  </ul>
</div>

{% include footer.html %}
