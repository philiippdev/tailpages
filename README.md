
gem install jekyll bundler
bundle install

bundle exec jekyll serve

```
NOTE: If this is your first time with Tailwind (just like me), you should know that Tailwind is “just-in-time”, i.e., Tailwind CSS is generated on-demand as you develop your html pages/templates instead of being generated in advance at initial build time. For example, if you specify content: ['./**/*.html'] in tailwind.config.js as shown above, the just-in-time engine scans all html files in this folder and generates the used styles into a tailwind output css file. For example, if you never used m-6 in any html file - it won’t be outputted into the file.
```


Then run `npx tailwindcss -i ./assets/css/main.css -o ./assets/css/tailwind.css --watch` to build the css file at ./assets/css/tailwind.css. --watch makes sure that the css is regenerated whenever a change is detected in HTML files.

# About

Tailpages (Tailwind + Github Pages) is a Jekyll website template based on TailwindCSS, which can be hosted by Github for free. You can visit the demo site at [https://harrywang.me/](https://harrywang.me/).

Key features are:

- Minimalist design inspired by the [indigo template](https://github.com/sergiokopplin/indigo)
- Elegant typography via [TailwindCSS Typography plugin](https://tailwindcss.com/docs/typography-plugin) and [Inter font](https://rsms.me/inter/)
- Markdown support for content authoring (static pages and blogs)
- Code highlighting and styling via [highlight.js](https://highlightjs.org/) (see [code example](http://harrywang.me/tailpages/2022/02/07/code.html))
- Latex support via [MathJax](https://www.mathjax.org/) (see an [example](http://harrywang.me/tailpages/2022/02/09/latex.html))
- Table of Contents support via [jekyll-toc](https://github.com/allejo/jekyll-toc) (see an [example](http://harrywang.me/tailpages/toc))

### Tutorials
- No-code Tutorial: this tutorial shows how you can use Tailpages template to quickly setup your website and blogs without coding, which you can access at [medium](https://harrywang.medium.com/introducing-tailpages-tailwind-github-pages-89903c52d3ec) or [blog](https://harrywang.me/tailpages-tutorial-nocode).
- Technical Tutorial: this tutorial shows how to setup the development environment for Tailpages from scratch, which you can access at [medium](https://harrywang.medium.com/developing-tailpages-a-jekyll-template-based-on-tailwind-css-b8b51e60e25b) or [blog](https://harrywang.me/tailpages-tutorial-technical). 
