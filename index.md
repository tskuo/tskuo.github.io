---
layout: bio
---

<div class="announcement">
  <b>On the job market for 2026–27</b>
  <p style="margin-bottom: 0px">I am seeking tenure-track faculty and research scientist positions!</p>
</div>

I am a final-year PhD candidate in the [Human-Computer Interaction Institute](https://www.hcii.cmu.edu/) at Carnegie Mellon University, co-advised by [Ken Holstein](https://kenholstein.com/) and [Haiyi Zhu](https://haiyizhu.com/), with a committee including [Amy X. Zhang](https://homes.cs.washington.edu/~axz/), [Niki Kittur](https://kittur.org/), and [Michael Bernstein](https://hci.stanford.edu/msb/). Currently, I am also a Student Researcher at Google DeepMind, working with [Michael Terry](https://research.google/people/107786/) and [Merrie Morris](https://research.google/people/meredithringelmorris/) in the [People + AI Research (PAIR)](https://pair.withgoogle.com/) Team.

I am a **human-computer interaction** researcher who combines system building, participatory design, and responsible AI. As AI impacts vital decisions across public agencies and online communities, I envision a future where AI is shaped by the people it serves, rather than external developers who lack the domain knowledge to address local needs. I build toward this future by **creating interactive systems that enable people to harness their collective intelligence for AI alignment**. Conversely, my systems also leverage AI to catalyze human collaboration, creating a virtuous cycle where collective _human_ intelligence and _artificial_ intelligence strengthen each other.

My interdisciplinary research has impact across academia, industry, and policy. My first-author papers have earned a **CHI Best Paper Award** and a **NeurIPS Spotlight**. I have been named both a [**Rising Star in ML & Systems**](https://mlcommons.org/about-us/programs/) and a [**Rising Star in Data Science**](https://datascience.uchicago.edu/research/postdoctoral-programs/rising-stars/). I was also selected by CMU as its [inaugural Fellow on AI & Society](https://www.cmu.edu/block-center/our-work/block-ai-society-fellowship) and [Presidential Fellow in Ethics & Computational Technologies](https://www.cmu.edu/ethics-ai/news/2025-fellows.html). Beyond academia, my work helped the [Wikimedia Foundation improve AI models](https://en.wikipedia.org/wiki/User:Tzusheng/sandbox/Wikipedia:Wikibench/Campaign:Editquality), inspired [Google's Kaggle to launch Community Benchmarks](https://blog.google/innovation-and-ai/technology/developers-tools/kaggle-community-benchmarks/), and informed policymaking at the [**European Parliament**](<https://www.europarl.europa.eu/RegData/etudes/STUD/2025/777915/IUST_STU(2025)777915_EN.pdf>) and [**White House OSTP**](https://www.whitehouse.gov/ostp/).

<!-- Previously, I hold an M.S. from Stanford University, where I worked with [James Landay](https://www.landay.org/) and [Elizabeth Murnane](https://engineering.dartmouth.edu/community/faculty/elizabeth-murnane) in the [Stanford HCI Group](https://hci.stanford.edu/). I also graduated summa cum laude in Electrical Engineering from [National Taiwan University](https://www.ntu.edu.tw/english/), as a [Phi Tau Phi Scholar](http://www.phitauphi.org.tw) and [Irving T. Ho Fellow](https://irvingthofoundation.github.io/ho-fellows.htm). -->

[&nbsp;[curriculum&nbsp;vitae](/assets/TzuShengKuo_CV.pdf)&nbsp;] [&nbsp;[research&nbsp;statement](/assets/TzuShengKuo_Research_Statement.pdf)&nbsp;] [&nbsp;[teaching&nbsp;statement](/assets/TzuShengKuo_Teaching_Statement.pdf)&nbsp;]

<div class="project-list-highlight">

  <h2><b>Main Research:</b> community-centered AI alignment through collective intelligence</h2>

  <!-- <h3>featured publications</h3> -->

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

## additional publications

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

## selected leadership

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
