## Portfolio Site (Using Github Pages)

This site functions as a portfolio of work and a small web side project.  This README should outline how to build and maintain the site locally.  New trunk builds will be published to github pages automatically.

### Local Setup

#### Notes on local builds

Github pages uses a slightly modified version of [jekyll](https://jekyllrb.com/).  Some things that work with github pages do *not* work with Jekyll locally.  Note that every page you want to add to the local build *must* have a [YAML front matter](https://jekyllrb.com/docs/front-matter/).  If a page doesn't have any variables to set, you must still add the front matter in the following format for the page to build correctly:

```yaml
---
---
```

#### Dependencies

You'll need the following installed to build locally:
* [Task](https://github.com/go-task/task) - a make replacement with friendlier syntax
* [Ruby](https://www.ruby-lang.org/en/) -A dynamic, open source programming language with a focus on simplicity and productivity
* [Jekyll](https://jekyllrb.com/) - a static site generator written in ruby
* [Bundle](https://bundler.io/) - a ruby dependency installer
* Gems for github pages and any themes you use with your site. These should be specified in a `Gemfile`

#### Install and build

Once you have the dependencies above installed, you can:

```bash
task install
task serve
```

This will install the required gems from the Gemfile and generate any static assets. Once done, you'll be able to view the locally built site on `http://localhost:4000`

```
