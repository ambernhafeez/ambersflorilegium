In Git Bash application cloned github repository to my local Documents/GitHub folder.
Installed Ruby with DevKit

In Git Bash:
` gem install jekyll bundler`

```
$ jekyll --version
jekyll 4.4.1
```

In GitHub folder:
`git clone https://github.com/mmistakes/minimal-mistakes.git minimal-mistakes`

Copy everything except the .github and README files into my website folder. Then, when in my website folder, install ruby gems:
`bundle install`

Then preview the site: `bundle exec jekyll serve`
looks ok!
In config.yaml, change name and description etc of website. 
Then make `_pages` folder and inside create any pages I need as `.md` files.

Create a `_pages` folder and inside `.md` files for each page.
Put headers like this in page files:

```
---

title: "About"

permalink: /about/

---
```

In `navigation.yml` put page names with urls:
```
# main links

main:

  - title: "About"

    url: /about/

  - title: "Blog"

    url: /blog/

  - title: "Florilegium Press: Audiobooks"

    url: /florilegium-press/

  - title: "Author Profile"

    url: /author-profile/

  - title: "Scientific Profile"

    url: /scientific-profile/

  - title: "Ambyte: Video Games"

    url: /ambyte-game-dev/

  - title: "Art"

    url: /art/

  - title: "Contact"

    url: /contact/
```

CSS 

```
/* remove sidebar */ 
---
layout: single
author_profile: false
---
```

