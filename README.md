# Untie Game Development
This is the website for Untie Game Development. It uses [jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll).


# Contributing
You can add new posts to the `docs/_posts` folder.  Make sure you follow the file name pattern.  See 
[github documentation](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll).

The pages can be made in markdown or html.  See markdown [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your 
[repository settings](https://github.com/Crennon-Dynamics/crennon-dynamics.github.io/settings/pages). 
The name of this theme is saved in the Jekyll `_config.yml` configuration file.


# Build and Run Locally
You can test the site locally at: http://127.0.0.1:4000/
```
$ bundle install
$ bundle exec jekyll serve
```


# Setup
The website depends on jekyll, which depends on ruby.  MacOS built in ruby in `usr/local/...` is
outdated and protected.  Use a different installation of ruby for your jekyll environment.  

### MacOS Installation with rbenv

```
# Install rbenv: (https://github.com/rbenv/rbenv#using-package-managers)

# install ruby via rbenv
$ rbenv install 3.1.1

# Set the global ruby version
$ rbenv global 3.1.1

# Verify the version is correct
$ rbenv versions
->   system
   * 3.1.1 (set by /Users/chrisatkeson/.rbenv/version)

# Restart your terminal (This is required for paths to be updated). 

# Check install paths
$ which ruby
-> /Users/chrisatkeson/.rbenv/shims/ruby

$ which gem
-> /Users/chrisatkeson/.rbenv/shims/gem

$ which jekyll
-> /Users/chrisatkeson/.rbenv/shims/jekyll

# check ruby version and environment
$ ruby --version
-> ruby 3.1.1p18 (2022-02-18 revision 53f5fc4236) [x86_64-darwin20]
$ gem env

# install bundler
$ gem install bundler

```

If your paths are not correct, follow these steps.

```
# Verify both .rbenv/shims and .rbenv/bin are in your path.  
$ echo $PATH
-> /Users/chrisatkeson/.rbenv/shims:/Users/chrisatkeson/.rbenv/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin

# Check your bash profile for rbenv path variables.  You should see them at the bottom of your profile.
$ cat ~/.bash_profile
-> export PATH="$HOME/.rbenv/bin:$PATH"
   eval "$(rbenv init -)"

# if these paths are missing, add them: 
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
$ echo 'eval "$(rbenv init -)"' >> ~/.bash_profile

# Restart your terminal and verify your path is correct.

```



# Github

You can use the [editor on GitHub](https://github.com/Crennon-Dynamics/crennon-dynamics.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
