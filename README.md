# Hugo YAMT Theme
**Y**et **A**nother **M**inimal **T**heme, inspired by <https://bestmotherfucking.website/>.

## Features
* Minimal and clean design
* Light & Dark Mode
* Somewhat responsive
* Simple blog & taxonomy system
* No JavaScript
* Small & fast

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
languageCode: en-US
title: <your_title>
theme: yamt

markup:
  goldmark:
    renderer:
      unsafe: true

params:
  author:
    email: <mail>
    gpgFingerprint: <fingerprint>
    name: <name>
    github: <link_to_your_github>
    address:
      street: <street>
      zipCode: <zip_code>
      city: <city>
      country: <country>
  hosting:
    name: <hosting_provider>
    address:
      street: <street>
      zipCode: <zip_code>
      city: <city>
      country: <country>
  description: <a_small_description_of_your_site>

defaultContentLanguage: <your_sites_main_language_code>
defaultContentLanguageInSubdir: true

languages:
  en:
    weight: 2
    languageName: English
    params:
      readingSpeed: 228
  de:
    weight: 1
    languageName: Deutsch
    params:
      readingSpeed: 179
```

Note that some options aren't strictly necessary, those are:
* `markup`:
  * `unsafe`: The unsafe renderer is required if you want to include html inside your markdown files
* `params`: Here contact & license information could be specified, this way links inside the header, footer
  & legal forms (imprint/privacy) are populated
