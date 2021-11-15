# Machine Learning for Science at Boston CollegeIAllan Lab Website

This is the website of an academic research group at Boston College.


## Data Editing
- Edit the `.yml` in `_data/`

## [Installation (Mac)](# Installation:  https://jekyllrb.com/docs/installation/macos/)
	- Install ruby
    ```
	brew install rbenv
	rbenv install 3.0.0
    # if using Bash
	echo 'export PATH="/usr/local/opt/ruby/bin:/usr/local/lib/ruby/gems/3.0.0/bin:$PATH"' >> ~/.bash_profilebrew install ruby
    rbenv global 3.0.0
    ```
	- Install jekyll
    ```
    gem install --user-install bundler jekyll
	bundle update --bundler
	gem install -n /usr/local/bin jekyll
	bundle add webrick
    ```

## [Local Dev](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)
```
cd PATH_TO_FOLDER/BC-ML4SCI/
bundle exec jekyll serve
```


Template from [Allan Lab](https://github.com/mpa139/allanlab)
Copyright ML4SCI@BC. Code released under the MIT License.
