---
layout: post
title:  "Documentation for this blog"
date:   2023-06-22
tags: jekyll blog documentation sample
date-updated: 2023-06-24
---

## About this theme
The theme is maintained [in a repo on my account](https://github.com/DeimosTheMisthios/no-style-please), forked from [someone else's theme of the same name](https://github.com/riggraz/no-style-please). The modifications include:
 - Addition of local [Katex v0.16.7](https://github.com/KaTeX/KaTeX/releases/tag/v0.16.7) (CSS/JS/font) files for rendering math on client side. I chose not to go with a CDN hosted version of Katex to have all scripts be hosted on the same domain.
 - A dark or light theme button in the top right, and the [associated JS file](/assets/js/mode-change.js). This was obtained from [another user's Github hosted portfolio](https://github.com/fleetimee/portfolio).
 - Minor changes like syntax highlighting for code blocks, removal of analytics and SEO plugin, changes to default fonts and code blocks.
 - Options to have [uppercase titles](https://github.com/riggraz/no-style-please/pull/21), [commentary appear above the archive page](https://github.com/riggraz/no-style-please/pull/22), [the index content appear on top](https://github.com/riggraz/no-style-please/pull/30), and [display update date in post](https://github.com/riggraz/no-style-please/pull/31).

## Creating a new post
Add a new post to the `_posts` folder with the name `YYYY-MM-DD-title.md`, with the [front matter](https://jekyllrb.com/docs/front-matter/) similar to that of this post. The URL used is the `title` from the file name, while the displayed title is sourced from the front matter. The site is tested locally using `bundle exec jekyll serve`, while Github pages deployments are available directly on the [home page](/).

## Sample elements
### Code
{% highlight ruby linenos %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

{% highlight python linenos %}
def print(name):
  print(f"Hi, {name}")
print_hi('Tom')
# prints 'Hi, Tom' to STDOUT.
def print(name):
  print(f"Hi, {name}")
print_hi('Tom')
# prints 'Hi, Tom' to STDOUT.
def print(name):
  print(f"Hi, {name}")
print_hi('Tom')
# prints 'Hi, Tom' to STDOUT.
def print(name):
  print(f"Hi, {name}")
print_hi('Tom')
# prints 'Hi, Tom' to STDOUT.
def print(name):
  print(f"Hi, {name}")
print_hi('Tom')
# prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

### Math / LaTeX
$$ \left[ \frac{-\hbar^2}{2\mu}\nabla^2 + V(\mathbf{r},t)\right] \Psi(\mathbf{r},t) $$

### Horizontal line
---

### Image that inverts with the theme
![Alt text](/favicon.ico "Tooltip text"){: .ioda width="20"}

### Image that doesn't invert
![Alt text](/favicon.ico "Tooltip text"){: width="20"}

### Table of contents
- [About this theme](#about-this-theme)
- [Creating a new post](#creating-a-new-post)
- [Sample elements](#sample-elements)
  - [Code](#code)
  - [Math / LaTeX](#math--latex)
  - [Horizontal line](#horizontal-line)
  - [Table of contents](#table-of-contents)
  - [Blockquote](#blockquote)
  - [Tables](#tables)
  - [Footnotes](#footnotes)

### Blockquote
The following is a blockquote:
> Fear is the response to loud noises, or loss of support.

### Tables

| Tables        | Are           | Cool  | Four |
| ------------- |:-------------:| -----:| :--: |
| col 3 is      | right-aligned | $1600 | one  |
| col 2 is      | centered      |   $12 | two  |
| zebra stripes | are neat      |    $1 | 3    |

### [Heading with title](#heading-with-title)
This is a reference for which a footnote is available below. [^1]

---
{: data-content="footnotes"}

[^1]: This is the source for that reference.