---
layout: post
title: "Hello World! (and info about Chalk, this blog template)"
description: "Every new skill we learn is a journey into a brave new world, so we must say hello (and give credit where credit is due)."
comments: True
tags: [personal]
---

In the throws of a stressful PhD, I've decided to start a blog. And so I say "Hello World!" as is customarily expected by any programmer. I plan to discuss random ideations when I feel like journaling while also creating a research journal of what I study each day to not only help me process what I read/work on but also practice my writing and communication skills. I'll probably alternate every other day or so on these two areas.

I tend to be open with my thoughts, which will often be a little blunt or risque sometimes. But I believe being my authentic self, especially in public, will not only help me in grappling with my own struggles and learning to overcome them, but will also help others in realizing that for at least one other person, they could be dealing with similar issues as them. Thus, I hope my experiences could impart some useful information to whomever takes the time to read this.

For instance I find myself to be depressed as of late for various reasons including not being as productive as I'd like to be and missing out on visiting friends because these additional years of grauate school takes over all my time and obligations, thus disallowing myself from being able to leave the campus at most times. It's the sacrifice I, and I believe most researchers, make as we pursue this path of enlightenment to understand the problems we are most passionate about.

What I think I can do differently, which I hope academic institutions will support and encourage more often, is to allow myself to take time off and escape from the walls of our offices/labs/minds and decompress with something completely different. Too often, especially in American culture, people like me guilt ourselves into working tirelessly while forgetting the simpler things in life like friends, staring at the sky, or a pickup soccer game. I don't want to be stuck in a constant loop of consumerist pursuit because in truth that is not what I want.

What I want from my work is an opportunity to understand how the universe and the environment around me works. But what I want for myself is simply to live contented, where I can be one with the people I share my life with while also being able to live in awe of the Earth we come from. Beauty can be found in the most simplest of things, but if I let the pursuit of work be corrupted by capitalist ideals, then I will miss out on just appreciating the moment. We don't always need to be looking forward to that next rung of the career ladder. Too much time spent planning on what we could be takes away from who we are in the now.

That's enough rambling on an opening post. I also need to give credit to the designer of this template. Learn more about this [Jekyll Chalk template here](https://github.com/nielsenramon/chalk).

Installing it was a little hard due to Windows and Cygwin never getting along and my noob experience with ruby in Linux, but I came through. It's only unfortunate that due to Github's limited compatibility with some plugins I'm using, I must manually build sites and upload to Github instead of just editting my markdown and pushing that (Github pages can build simple Jekyll sites automatically). Learn about Jekyll [here](https://jekyllrb.com/).

<br><br><br>
Lastly, I'm including all the original content of this Chalk template introduction content below to maintain a record (and serve as manual to you) if you wish to recreate smething like this site for yourself.

## Introducing Chalk

{% include image.html path="documentation/chalk-intro.png" path-detail="documentation/chalk-intro@2x.png" alt="Chalk intro" %}

[Download Chalk here!](https://github.com/nielsenramon/chalk)

#### Features:
  - Dark and Light theme.
  - Filter on tags.
  - Customizable pagination.
  - Beautified link sharing in Facebook and other social media.
  - Automatic time to read post indicator.
  - Automatic RSS feed.
  - About page.
  - 404 page.
  - SEO optimized.
  - PageSpeed optimized.
  - Cross browser support (supports all modern browsers).
  - Media embed for videos.
  - Enlarge images on click (like Medium).

#### Integrations
  - [Google Analytics](https://analytics.google.com/analytics/web/)
  - [Google Fonts](https://fonts.google.com/)
  - [Disqus](https://disqus.com/)
  - [Ionicons](http://ionicons.com/)
  - Social media links

#### Used tools
  - [Autoprefixer](https://github.com/postcss/autoprefixer)
  - [Bower](http://bower.io/)
  - [Circle CI](https://circleci.com/)
  - [Html-proofer](https://github.com/gjtorikian/html-proofer)
  - [Jekyll](http://jekyllrb.com/)
  - [Jekyll assets](https://github.com/jekyll/jekyll-assets)
  - [Jekyll Sitemap](https://github.com/jekyll/jekyll-sitemap)
  - [HTML5 Boilerplate](https://html5boilerplate.com/) (Influenced by)
  - [Kickster](http://kickster.nielsenramon.com/)
  - [Retina.js](http://imulus.github.io/retinajs/)
  - [STACSS](http://stacss.nielsenramon.com/)

{% include image.html path="documentation/enlarge.gif" path-detail="documentation/enlarge@2x.gif" alt="Enlarge image feature" %}

## Installation

If you haven't installed the following tools then go ahead and do so (make sure you have [Homebrew](http://brew.sh/) installed):

{% highlight bash %}
brew install ruby
brew install npm
{% endhighlight %}

Next setup your environment:

{% highlight bash %}
bin/setup
{% endhighlight %}

## Development

Run Jekyll:

{% highlight bash %}
bundle exec jekyll serve
{% endhighlight %}

## Deploy to GitHub Pages

Run this in the root project folder in your console:

{% highlight bash %}
bin/deploy
{% endhighlight %}

You can find more info on how to use the gh-pages branch and a custom domain [here](https://help.github.com/articles/quick-start-setting-up-a-custom-domain/).

[View this](https://github.com/nielsenramon/kickster#automated-deployment-with-circle-ci) for more info about automated deployment with Circle CI.

_If you have any questions about using or configuring Chalk please create an issue <a href="" title="here" target="_blank">here</a>!_

## How to Configure Chalk


The `_config.yml` file is the most important one. It contains the basic setup of your project.
Some parts are preconfigured and shouldn't be touched as the comments state.
Of course if you are familiar with Jekyll you can change whatever you want.

Note: You do not _have_ to change anything. Chalk works out of the box. I do recommend changing the `_config.yml` to suit your needs.

### Mandatory settings

{% highlight yml %}
# Mandatory settings

baseurl: /
name: Chalk
paginate: 25
paginate_path: "/posts/page/:num/"
url: http://chalk.nielsenramon.com # add site url http://example.com/
blog_theme: light # Or use dark
{% endhighlight %}

* `baseurl`: Set baseurl to match the production URL without the host.
* `name`: Used as the page title and throughout your project as the default name.
* `paginate`: Define how much posts should be shown on the homepage for each page.
* `paginate_path`: Change the path name to something else for paginated pages.
* `url`: Your production url (http://example.com).
* `blog_theme`: 2 options here, `light` or `dark`. Choose which design you prefer.

### Optional settings

{% highlight yml %}
# Optional settings

discus_identifier: # Add your Disqus identifier
ga_analytics: # Add your GA Tracking Id
rss_enabled: true # Change to false if not
social:
  dribbble: # Add your Dribbble link
  facebook: # Add your Facebook link
  github: # Add your GitHub link
  linkedin: # Add your LinkedIn link
  twitter: # Add your Twitter handle
{% endhighlight %}

* `discus_identifier`: If you like to use Disqus for comments on each blog post, you can add the Disqus identifier here and it will popup automatically.
* `ga_analytics`: Add Google Analytics Tracking ID here.
* `rss_enabled`: When set to `true`, the rss icon in the top navigation will show up and people will be able to subscribe to your rss feed.
* `social`: Add you social links in here. When filled in they will show up in the navigation.

### Other settings

Other than the `_config.yml` you can change a lot more in the project.

#### Tags

To add tags you must add a file with the tag name in `_my_tags`.
In the file you add 2 variables: `slug` used to reference the tag and `name` which is displayed in the article header.

{% highlight yml %}
# _my_tags/design.md
---
slug: design
name: Design
---
{% endhighlight %}

#### SCSS

You can change colors, fonts, sizes in the `_assets/stylesheets/_variables.scss` file.
For each specific theme (light or dark) you can change the variables in `_assets/stylesheets/dark.scss` and `_assets/stylesheets/light.scss`.

{% highlight scss %}
// =============================================================================
// Variables
// =============================================================================

// Typography
// =============================================================================

$sans-serif: "Lato", Helvetica, Arial, sans-serif;
$serif: "Cormorant Garamond", Courier, serif;
$base-font-family: $sans-serif;
$base-font-weight: 400;
$base-font-weight-bold: 700;

// Colors
// =============================================================================

// Brand colors

$brand-success: #1fbf92;
$brand-danger: #e74b3c;
$brand-primary: #3449ed;
$brand-warning: #f1c90b;

// Sizes
// =============================================================================

// Grid

$columns: 12;
$max-width: 650px;
$gutter: 20px;
$one-column: 100% / $columns;
$negative-gutter: 0 - $gutter;

// Font sizes

$base-font-size: 16px;
$base-line-height: 1.8;

// Box sizes

$base-border-radius: 4px;

// Effects
// =============================================================================

$base-transition-speed: .2s;
{% endhighlight %}

#### Fonts

Chalk uses Google Fonts by default. You can change the font in `_includes/javascripts.html`.

{% highlight html %}
<script src="https://ajax.googleapis.com/ajax/libs/webfont/1.6.16/webfont.js"></script>
<script>
  WebFont.load({
    google: {
      families: ['Cormorant Garamond:700', 'Lato:300,400,700']
    }
  });
</script>
{% endhighlight %}

#### Footer

Changing the text in the footer is easy. It can be found in `_includes/footer.html`.

_If you have any questions about using or configuring Chalk please create an issue <a href="" title="here" target="_blank">here</a>!_

## Chalk Sample Post with All the Elements

Chalk uses the default Jekyll syntax highlighting gem Rouge. It has a customized style for both light and dark theme.
Use the `highlight` tag to use the following code highlighting your preferred language:

{% highlight html %}
<!-- This is a comment -->
<div class="grid">
  <h1>This is a heading</h1>
  <p>
    This is a paragraph text.
  </p>
</div>
{% endhighlight %}

## Headings

Chalk includes 3 headings by default:

## Heading first level
### Heading second level
#### Heading third level

{% highlight markdown %}
## Heading first level
### Heading second level
#### Heading third level
{% endhighlight %}

## Lists

Unordered list example:
* Unordered list item 1
* Unordered list item 2
* Unordered list item 3
* Unordered list item 4

Ordered list example:
1. Ordered list item 1
2. Ordered list item 1
3. Ordered list item 1
4. Ordered list item 1

{% highlight markdown %}
* Unordered list item 1
* Unordered list item 2

1. Order list item 1
2. Order list item 1
{% endhighlight %}

## Emoji support :star:

Emoji's can be used everywhere in :cat2: your markdown!

## Quotes

A quote looks like this:

> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.

{% highlight markdown %}
> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna.
{% endhighlight %}

## Media

Images can be added with a default `<img>` tag.
If you wish that an image can be enlarged on click use the image include tag. You can pass 3 variables:
- `path`: Image to show in the blog post.
- `path-detail`: Image to show when enlarging.
- `alt`: Alt text for image in blog post.

{% include image.html path="documentation/sample-image.jpg" path-detail="documentation/sample-image@2x.jpg" alt="Sample image" %}

{% highlight html %}
{% include image.html path="documentation/sample-image.jpg" path-detail="documentation/sample-image@2x.jpg" alt="Sample image" %}
{% endhighlight %}

Videos can be added and are responsive by default (4x3 by default, 16x9 with extra class).

<div class="embed-responsive embed-responsive-16by9">
<iframe src="https://www.youtube.com/embed/vO7m8Hre72E?modestbranding=1&autohide=1&showinfo=0&controls=0" frameborder="0" allowfullscreen></iframe>
</div>

{% highlight html %}
<div class="embed-responsive embed-responsive-16by9">
<iframe src="url-to-video" frameborder="0" allowfullscreen></iframe>
</div>
{% endhighlight %}