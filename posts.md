# Create a Post
We encourage you to create a post of a topic. Follow these steps:

Install [Hugo](https://gohugo.io/getting-started/installing/)

* step 0: Fork the project
* step 1: Clone your fork
* step 2: `cd src`
* step 3: `hugo new posts/<name>.md`

with these steps you can go to `src/content/posts` and there will be your template for your post.

You will have to create a summary of the post, it has to be before the tag `<!--more-->`. After that tag you can start your post.

Before creating a new `tag` or `category` PLEASE make sure that it already exists and use one that exists. If it is not the case then create it and specify on the pull request.

## Template
* title (name of the file)
* date (autogenerated)
* draft (false)
* author [change]
* year (autogenerated)
* month (autogenerated)
* categories: you can create a category or [use](https://0xbuilders.github.io/categories/)
* tags: you can create a category or [use](https://0xbuilders.github.io/tags/)

## Publish post
To publish the post you will have to create a pull request to `posts` branch specifying any new categories or tags created, author and a summary.
