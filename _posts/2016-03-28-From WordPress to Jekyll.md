---
layout: post
title: From WordPress to Jekyll
---

This week I relaunched this site as a static Jekyll site. When I first developed my site in 2014 I used WordPress. After assessing my needs I realized WordPress was a more powerful and complicated solution than I required for a site to blog and post links to my latest projects. Below are the top three reasons I chose to replace my WP site with a static site.

## 1. Simplicity
Being the sole content creator of this site and a programmer, I don't have a need for a content management system (CMS). I dont need a CMS and a database for a site of text and images.

## 2. Markdown
Text files suited my needs and I prefer using them for writing. I can write my posts offline in Markdown and instead of the WP WYSIWYG and HTML editor for post writing.

## 3. Free Hosting on GitHub
Hosting my site for free using [GitHub Pages](https://pages.github.com/) saved the hosting fee I was paying. Version control with Git is another bonus. And, because I have a local and remote repo for my site I have a backup if needed.

## Jekyll vs Pelican
After deciding to go static, I reviewed the options for static site generators on [StaticGen](https://www.staticgen.com/ ) and narrowed by options to Jekyll and Pelican. Jekyll has the advantage of being synonymous with static sites and GitHub pages friendly. It is also written in Ruby and that appealed to me since I am learning Ruby now. The downside of Jekyll is the lack of official support for Windows, which makes getting set up more complicated for me. Pelican appealed to me because it's written in Python. I have more experience with Python and it's a fun language I enjoy working with. Plus, I already have Python set up and the experience on Windows has been almost painless. The downside of Pelican is that it is more complicated to get it set up to be hosted on GitHub pages because of the site generating to an output folder. 

I tried Pelican first and found it difficult to implement the workaround to get only the output folder to commit to the master branch of my repository. Implementing the automated script to do this was more complicated in Windows as well. So, I switched to Jekyll, installed an open source theme to save time on design, and loaded posts from my WP site. For projects, I redid my project page from WordPress from scratch in a new page layout in Jekyll.

## Tips for Converting from WordPress
1. Backup your WordPress site and use the Jekyll plugin. I didn't did not do this and it would have made the process of getting my site finalized once Jekyll was set up more efficient.

2. Choose themes carefully. Some themes are more complicated than others and can be intimidating for first time static site users. If you are new to static sites or Jekyll, pick a simple theme. One possible indicator of the complexity of a theme is its _config.yml file. The more complicated a theme the more custom configurations there will be that you will have to learn what they mean and how they work.

3. Use documentation or a tutorial. I did both using the official Jekyll documentation and the Treehouse course [Build a Blog with Jekyll and GitHub Pages](https://teamtreehouse.com/library/build-a-blog-with-jekyll-and-github-pages). Reading through documentation or following a course will help you understand Jekyll behind the scences and allow you to implement the design and functionality you envision more easily.

4. Build locally first. Set up and build your site on your computer and serve it to localhost to view it until you are satisfied with it. Initialize your git repository then create your GitHub repository online, if you are hosting on GitHub. This will allow you to maintain your site locally then push it to GitHub using it as your production server.


## Conclusion
So far, Jekyll seems to be the right solution for a static site generator and would recommend it. For Pythonistas (or loyal Python fans that go by other monikers) give Pelican a try-especially if you are not using GitHub pages and Windows. Overall, I am happy with the converstion from a WordPress site to a static site. It's a viable option for basic sites with content creators comfortable with the command line.