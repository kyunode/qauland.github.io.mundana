# qauland.github.io

Based on [Mundana Jekyll Theme by WowThemes.net](https://bootstrapstarter.com/bootstrap-templates/mundana-theme-jekyll/).

[Live Demo](https://wowthemesnet.github.io/mundana-theme-jekyll/) &nbsp; | &nbsp; 
[Download](https://github.com/wowthemesnet/mundana-theme-jekyll/archive/master.zip) &nbsp; | &nbsp; 
[Buy me a coffe](https://www.wowthemes.net/donate/) &nbsp; | &nbsp; [Documentation](https://bootstrapstarter.com/bootstrap-templates/mundana-theme-jekyll/) &nbsp; | &nbsp; 
[WordPress version](https://www.wowthemes.net/themes/mundana-wordpress/) 

![mundana jekyll theme screenshot](assets/images/screenshot.jpg)

### Contribute to Mundana repository

1. In the top-right corner of this page, click **Fork**.

2. Clone a copy of your fork on your local, replacing *YOUR-USERNAME* with your Github username.

   `git clone https://github.com/YOUR-USERNAME/mundana-theme-jekyll.git`

3. **Create a branch**: 

   `git checkout -b <my-new-feature-or-fix>`

4. **Make necessary changes and commit those changes**:

   `git add .`

   `git commit -m "new feature or fix"`

5. **Push changes**, replacing `<add-your-branch-name>` with the name of the branch you created earlier at step #3. :

   `git push origin <add-your-branch-name>`

6. Submit your changes for review. Go to your repository on GitHub, you'll see a **Compare & pull request** button. Click on that button. Now submit the pull request.

That's it! Soon I'll be merging your changes into the master branch of this project. You will get a notification email once the changes have been merged. Thank you for your contribution.


### Copyright

Copyright (C) 2019 WowThemes.net.

Theme designed and developed by [Sal](https://www.wowthemes.net), *free* under MIT license. 

<a href="https://www.wowthemes.net/donate/" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>

### Live Demo

[Live Demo](https://wowthemesnet.github.io/mundana-theme-jekyll/)

### Deleted codes

```html
<!-- Begin post excerpts, let's highlight the first 4 posts on top -->
<div class="row remove-site-content-margin">
    
    <!-- latest post -->
    {% assign latest_post = site.posts[0] %}
    <div class="col-md-6">
    <div class="card border-0 mb-4 box-shadow">   
    <a href="{{site.baseurl}}{{latest_post.url}}">
    <div class="topfirstimage" style="background-image: url({% if latest_post.image contains "://" %}{{ latest_post.image }}{% else %} {{site.baseurl}}/{{ latest_post.image}}{% endif %}); height: 200px;    background-size: cover;    background-repeat: no-repeat;"></div>     
    </a>
    <div class="card-body px-0 pb-0 d-flex flex-column align-items-start">
    <h2 class="h4 font-weight-bold">
    <a class="text-dark" href="{{site.baseurl}}{{latest_post.url}}">{{ latest_post.title }}</a>
    </h2>
    <p class="excerpt">
        {{ latest_post.excerpt | strip_html | strip_newlines | truncate: 136 }}
    </p>
    <div>
        <small class="d-block text-muted">
            In <span class="catlist">
                {% for category in latest_post.categories %}
                <a class="text-capitalize text-muted smoothscroll" href="{{site.baseurl}}/categories.html#{{ category | downcase }}">{{ category }}</a><span class="sep">, </span>
                {% endfor %}
                </span>                   
        </small>
        <small class="text-muted">
            {{ latest_post.date | date: '%b %d, %Y' }}
        </small>
    </div>
    </div>
    </div>
    </div>
    
    <div class="col-md-6">
        
        <!-- second latest post -->
        {%- assign second_post = site.posts[1] -%}        
        <div class="mb-3 d-flex align-items-center">                
                {% if second_post.image %}
                <div class="col-md-4">
                <a href="{{site.baseurl}}{{second_post.url}}">
                 <img class="w-100" src="{% if second_post.image contains "://" %}{{ second_post.image }}{% else %}{{ second_post.image | absolute_url }}{% endif %}" alt="{{ second_post.title }}">
                </a>
                </div>
                {% endif %}                
                <div>
                    <h2 class="mb-2 h6 font-weight-bold">
                    <a class="text-dark" href="{{site.baseurl}}{{second_post.url}}">{{ second_post.title }}</a>
                    </h2>
                    <small class="d-block text-muted">
                        In <span class="catlist">
                        {% for category in second_post.categories %}
                        <a class="text-capitalize text-muted smoothscroll" href="{{site.baseurl}}/categories.html#{{ category | downcase }}">{{ category }}</a><span class="sep">, </span>
                        {% endfor %}
                        </span>                   
                    </small>
                    <small class="text-muted">
                        {{ second_post.date | date: '%b %d, %Y' }}
                    </small>
                </div>
            </div>
        
        <!-- third latest post -->
        {%- assign third_post = site.posts[2] -%}        
        <div class="mb-3 d-flex align-items-center">                
                {% if third_post.image %}
                <div class="col-md-4">
                <a href="{{site.baseurl}}{{third_post.url}}">
                 <img class="w-100" src="{% if third_post.image contains "://" %}{{ third_post.image }}{% else %}{{site.baseurl}}/{{ third_post.image }}{% endif %}" alt="{{ third_post.title }}">
                </a>
                </div>
                {% endif %}                
                <div>
                    <h2 class="mb-2 h6 font-weight-bold">
                    <a class="text-dark" href="{{site.baseurl}}{{third_post.url}}">{{ third_post.title }}</a>
                    </h2>
                    <small class="d-block text-muted">
                        In <span class="catlist">
                        {% for category in third_post.categories %}
                        <a class="text-capitalize text-muted smoothscroll" href="{{site.baseurl}}/categories.html#{{ category | downcase }}">{{ category }}</a><span class="sep">, </span>
                        {% endfor %}
                        </span>                   
                    </small>
                    <small class="text-muted">
                        {{ third_post.date | date: '%b %d, %Y' }}
                    </small>
                </div>
            </div>
        
        <!-- fourth latest post -->
        {%- assign fourth_post = site.posts[3] -%}        
        <div class="mb-3 d-flex align-items-center">                
                {% if fourth_post.image %}
                <div class="col-md-4">
                <a href="{{site.baseurl}}{{fourth_post.url}}">
                <img class="w-100" src="{% if fourth_post.image contains "://" %}{{ fourth_post.image }}{% else %}{{site.baseurl}}/{{ fourth_post.image }}{% endif %}" alt="{{ fourth_post.title }}">
                </a>
                </div>
                {% endif %}                
                <div>
                    <h2 class="mb-2 h6 font-weight-bold">
                    <a class="text-dark" href="{{site.baseurl}}{{fourth_post.url}}">{{ fourth_post.title }}</a>
                    </h2>
                    <small class="d-block text-muted">
                        In <span class="catlist">
                        {% for category in fourth_post.categories %}
                        <a class="text-capitalize text-muted smoothscroll" href="{{site.baseurl}}/categories.html#{{ category | downcase }}">{{ category }}</a><span class="sep">, </span>
                        {% endfor %}
                        </span>                   
                    </small>
                    <small class="text-muted">
                        {{ fourth_post.date | date: '%b %d, %Y' }}
                    </small>
                </div>
            </div>
        
    </div>
    
</div>
```
