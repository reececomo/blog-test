# HealthEngine Engineering

Powered by [Kube+Hugo](https://themes.gohugo.io/kube/).

## Deploy

Deploy using the script `deploy.sh "Your optional commit message"` (full guide available [here](https://gohugo.io/hosting-and-deployment/hosting-on-github/)).

This will need to be adjusted for pull requests.

## Installation

```bash
# Install Hugo
brew install hugo

# Clone the repo
git clone https://github.com/healthengineau/blog.git

# Start the webserver
hugo server -w
```

## Adding Content

### Creating Blog Posts

You can add multiple content types (see **Configuring the Website**), but you'll want to use the `blog` type (nested inside the `blogs` directory). It's best to date them (year-month-day), purely so they appear neatly in order on GitHub.

Creating
```bash
hugo new --kind blog blog/2020-03-24-my-awesome-new-blog.md
```

### Front Matter

Each blog is generated with a snippet of metadata called **Front Matter**. For example:

```
+++
title = ""
description = ""
date = 2019-07-18T14:53:26+08:00
weight = 20
draft = false
+++

```

You'll need to fill out the:
- `title`
- `description`

and optionally you'll want to add yourself as the author: `author = "Your Name"`

## Configuring the Website

### Creating Docs
```bash
hugo new --kind docs docs/my-new-doc.md
```

### Other
Other supported types are:
- `faq` - Frequently Asked Questions
- `company` - Information about the company
- `sign-in` - This one's pretty obvious

## Index Blocking, Custom CSS and More

Please read https://themes.gohugo.io/kube/ for full details on how to configure
