# Hugo YAMT Theme
**Y**et **A**nother **M**inimal **T**heme, inspired by <https://bestmotherfucking.website/>.

## Features
* Minimal and clean design
* Light & Dark Mode
* Somewhat responsive
* Simple blog & taxonomy system
* No JavaScript
* Small & fast

## Requirements
* [Hugo](https://github.com/gohugoio/hugo) 0.148 or higher (lower might also work, but haven't tested)

## Installation
Install it as a git submodule inside the root of your Hugo project:
```
git submodule add https://github.com/ckiri/yamt.git themes/yamt
```

Add the theme to your sites configuration `hugo.yaml` in required format:
```yaml
theme: yamt
```

## Configuration

Configuration for your site (again in `hugo.yaml`) **should/could** contain the following options:
```yaml
baseURL: https://<your_domain>/
languageCode: en-EN
title: <your_websites_title>

menus:
  main:
    - name: Home
      pageRef: /
      weight: 10
    - name: Blog
      pageRef: /posts
      weight: 20
    - name: Tags
      pageRef: /tags
      weight: 30

markup:
  goldmark:
    renderer:
      unsafe: true
    extensions:
      passthrough:
        delimiters:
          block:
          - - \[
            - \]
          inline:
          - - \(
            - \)
        enable: true

params:
  author:
    email: <your_email>
    name: <your_name>
    github: <link_to_your_github>
  license:
    content: CC BY-SA 4.0
    contentRef: https://creativecommons.org/licenses/by-sa/4.0/
```

Note that some options aren't strictly necessary, those are:
* `markup`:
  * `unsafe`: The unsafe renderer is required if you want to include html inside your markdown files
  * `passthrough`: This allows you to write mathmatical expressions using `\(` `\)` for inline
    & `\[` `\]` for blocks. It uses Hugos integrated \(\KaTeX\) rendering engine, so no client-side javascript
    is required.
* `params`: Here contact & license information could be specified, this way links inside the header & footer are populated
