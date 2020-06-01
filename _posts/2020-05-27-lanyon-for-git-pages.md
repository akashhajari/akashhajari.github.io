---
layout: post
title: Lanyon for Github Pages
permalink: blogs/Lanyon-for-Github-Pages
comments_id: 1
---

Github Pages provide awesome provision for hosting your blog, personal website, etc.
There are many cool themes. I found Lanyon as coolest theme. It proides information/blog first with toggling sidebar.

### First part lets install jekyll for you desktop. 
I am using Ubuntu 16.04.
Update Ruby to 2.4 or later. Ubuntu16.04 has version 2.2 but can be upgraded to suggested upper version 2.4 :
* ```sudo apt-add-repository ppa:brightbox/ruby-ng```
* ```sudo apt-get update```
* ```sudo apt-get install ruby2.4```
* ```sudo apt-get install ruby`ruby -e 'puts RUBY_VERSION[/\d+\.\d+/]'`-dev```
* ```sudo gem update --system```
* ```echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc```
* ```echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc```
* ```echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc```
* ```source ~/.bashrc```
* ```gem install jekyll bundler```

### Then its time to use theme. 
Clone the [Lanyon Github repo](https://github.com/poole/lanyon.git)
* There no default gemfile by default in its [Github repo](https://github.com/poole/lanyon.git). So, I took one from [Poole Github repository](https://github.com/poole/poole.git) and copied it there.
* ```bundle install```
* If there are still error regarding sass-converter
  ```gem install jekyll jekyll-gist jekyll-sitemap jekyll-seo-tag jekyll-paginate  jekyll-sass-converter```
* ```bundle exec jekyll serve```
* Cool! Access you site locally at http://127.0.0.1:4000/
* You need to check _config.yml file, _posts folder for writting your posts :) . For customisation you can check index.html, includes/ , public/csv/ etc. Don’t forget to read README.md.
* Then you can upload all the content to your github repository where you would be publishing your static site. There are plenty of tutorials available on this.

Thanks!
