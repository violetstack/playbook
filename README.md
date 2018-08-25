# The Violet Stack playbook

We're using Jekyll for a few reasons:

- We all love contributing via git
- Super easy to get up and running
- Static hosting is fast
- Makes it simple to manage relatively static content (no need for CMS)

To get up and running:

1. Pull down the repo
2. Make sure Jekyll is installed `gem install jekyll`
3. run `jekyll serve` and boom, it should be available at `http://localhost:4000`

To add a new post:

1. Head to the `_posts` folder
2. Create a new post. Directory structure is for organization purposes only— it
doesn't impact the URL since we use the `permalink` page property in each post.
3. Make sure it has a date appended to the front, e.g. `2018-08-24-name-of-post.md`
4. You can have it as a `.html` or `.md`, and the Markdown format supports html
so that's our preferred method

---

#### Note on URL paths
We're using **absolute** paths for assets because we're nesting content
inside nicer permalinks (e.g. `/company/sales`), and Jekyll doesn't have
a nice relative path handler built-in. This means if you run this in a sub-directory
like GitHub pages does (e.g. `violetstack.github.io/playbook/`), it'll break.
Just make sure you're running this in it's own subdomain and you'll be fine.
For more about Jekyll + paths, [check this post out.](https://ricostacruz.com/til/relative-paths-in-jekyll)
