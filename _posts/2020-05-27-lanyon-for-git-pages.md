---
layout: post
title: Lanyon for Github Pages
---

Github Pages provide awesome provision for hosting your blog, personal website, etc.
There are many cool themes. I found Lanyon as cool theme. It proides information/blog first with toggling sidebar.

### First part lets install jekyll in you desktop. 
I am using Ubuntu 16.04.
Update Ruby to 2.4 or later. Ubuntu16.04 by dafalut ships with 2.2 but has maximum support for 2.4 :
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
* You need to check _config.yml file, _posts folder for writting your posts :) . For customisation you can check index.html, includes folder, etc. Don’t forget to read README.md.
* You can make custom changes in 
* Then you you can upload the all the content to your github repository where you would be publishing your static site. There are plenty og these tutorials available on this.

Thanks!

Let me know if you have any questions or feedback on [Twitter]({{site.author.twitter}}) or [LinkedIn]({{site.author.linkedin}})
