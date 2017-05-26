## My Personal Website
This project is based on Beautifull-jekyll project, if you like tis template, please clone from the original one and support him to maintain it.

## Local Testing on Arch linux

To test locally you will need ruby with github-pages and jekyll gems

```
	$ gem install github-pages jekyll
	$ gem install bundler
	$ gem update
```

There are a few things to do before testing locally, you have to add the following lines to your bashrc file to prevent 
gems to work without having to input the full location and to prevent bundler to install gems system wide, rspectively:

```
	PATH="$(ruby -e 'print Gem.user_dir')/bin:$PATH"
	export GEM_HOME=$(ruby -e 'print Gem.user_dir')

```
Then you need to install the required gems of this website project by executing:

```
	$ bundler install
```

So after installing everything needed you can build your website with:

```
	$ bundler exec jekyll serve
```
And access it on:

```
	http://localhost:4000
```
