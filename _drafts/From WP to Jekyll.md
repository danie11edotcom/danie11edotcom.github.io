---
layout: post
title: From WordPress to Jekyll
---

This week I changed this site from a dynamic WordPress (WP) site to a static Jekyll site. WordPress is a powerful tool for blogging and websites in general especially for teams or multiple users adding and editing content. At the time I set up my site in 2014, WP was the best choice for use because I was learning WP and considering becoming a WP developer. Building my site locally and transferring it to my site's server was great hands on practice and experience. Since then my goals have changed and I've transitioned from learning WP to learning JavaScript, Python and now Ruby. My site was due for a redesign and a new blog post. After assessing my needs I realized WP was more powerful and complicated solution than I required for a site to blog and post links to my latest projects. Below are the top three reasons I chose to replace my WP site with a static site.

## Simplicity
I didnt' require a content management system and a database to write blogs and projet descriptions. Text files were suitable.

## Markdown
I can write my posts offline in Markdown and ditch the WP WYSIWYG and HTML editor for post writing. I never liked those.

## Free Hosting on GitHub
Hosting my site for free using [GitHub Pages](https://pages.github.com/) saved the hosting cost I was paying. Version control with Git is another bonus. And, because I have a local and remote repo for my site I have a backup if needed.

## Jekyll vs Pelican
After deciding to go static I reviewed the options for static site generators on [StaticGen](https://www.staticgen.com/ ) and narrowed by options to Jekyll and Pelican. Jekyll has the advantage of being synonymous with static sites and GitHub pages friendly. It is also written in Ruby and the chance to work with a Ruby project apealled to me since I am learning Ruby now. The downside of Jekyll is the lack of official support for Windows, which makes getting set up more complicated for me. Pelican appealed to me because it's written in Python. I have more experience with Python and it's a fun language I enjoy working with. Plus, I already have Python set up and the experience on Windows has been almost painless. The downside of Pelican is that is more complicated to get it set up to be hosted on GitHub. Pelican's site generates in an output file. 

I tried Pelican first and found it difficult to implement the workaround to get only the output folder to commit to the master branch. Implementing the automated script to do this was more complicated in Windows as well. So I switched to Jekyll, installed an open source theme to save time on design and loaded posts from my WP site. For projects I redid my project page from WP from scratch in a new page layout in Jekyll.

## Tips for Converting from WordPress
1. Backup your WP site and use the Jekyll plugin. I didn't did not do this and it would have made the process of getting my site finalized once Jekyll was set up more efficient.

2. Choose themes carefully. Some themes are more complicated than others and can be more intimidating for first time static site users. If your new to static sites or Jekyll pick a simple theme to begin with. Once indicator of the complexity of a theme is its _config.yml file. The more complicated a theme the more custom configurations there will be that you will have to learn what they mean and how they work.

3. Use the documentation or a tutorial. I did both using the official Jekyll documentation and the Treehouse course [Build a Blog with Jekyll and GitHub Pages](https://teamtreehouse.com/library/build-a-blog-with-jekyll-and-github-pages). Reading through documentation or following a course will help you understand Jekyll behind the scences and allow you to implement the design and functionality you envision more easily.

4. Build locally first. Set up and build your site on your computer and serve it to localhost to view it until you are satisfied with it. Initialize your git repo then reate your GitHub repo online, if you are hosting on GitHub, then use that to push your local repo. That way you can maintnain your site locally then push it to the GitHub using it as your production server.


## Conclusion
This article is the first I have written using Markdown and I already like it better. Overall I am happy with the swith and would recommend Jeykll. For Pythonista's not using GitHub and Windows I would recommend Pelican. If I can't had such difficulty and got my site up on the first try, I wouldn't have tried Jekyll for this project. In general I recommend static sites for projects where a writing and images are the primary content, for authors comfortable with the command line.