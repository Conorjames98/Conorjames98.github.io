+++
date = '2024-11-22T00:27:57Z'
draft = false
title = 'A blog with hugo'
+++

# Making a blog with Hugo and Github pages.

Firstly Hugo need's to be installed depending on the OS you're running 

### Windows
Refer to: https://gohugo.io/installation/windows/

This tutorial will guide you through the installation on Windows

### Mac
Refer to: https://gohugo.io/installation/macos/

This tutorial will guide you through the installation on Mac

## Creating a hugo site

Open a terminal and use:

```bash
------------------------------------------------------
hugo new site quickstart
cd quickstart
git init
git submodule add
<Your submodule>
echo "theme = 'ananke'" >> hugo.toml
hugo server
------------------------------------------------------
```

## How to add new content to your new site

Hugo new content content/posts/my-first-post.md
<!--more-->

Hugo created the file in the content/posts directory. Open the file with your editor.

Your first post will look like this:

```bash
+++
title = 'My First Post'
date = 2024-01-14T07:07:07+01:00
draft = true
+++
```






