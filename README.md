# mondesinxi.github.io
Personal site that I use to document everything that I come accross that could be useful to anyone 

## Getting started

### Installing Hugo
I use Hugo to generate a static site. I'll go through a quick installation procedure.
Download [from source](https://github.com/gohugoio/hugo/releases)

`wget https://github.com/gohugoio/hugo/releases/download/v0.55.6/hugo_0.55.6_Linux-64bit.deb`

then 

`sudo dpkg -i /path/to/deb/file`

finally install 

`sudo apt-get install -f`

This should be working.

### Setting up the new site

Lets create the directory structure for the blog site

`hugo new site blog`

Inside this directory download a there
```
cd blog

git init

git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke

echo 'theme = "ananke"' >> config.toml
```

Then we can add new content

`hugo new posts/getting-started-with-fastai.md`

Change the title in the `config.toml` file


### Publishing our site

run `./deploy.sh "message" to publish

`
