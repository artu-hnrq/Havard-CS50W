# Project 0: Search
*[Harvard CS50W Course][1]*

This project requires the development of a static website, resembling google search.
Throughout it, student's knowledge of several HTML elements usage, as well as its styling,
and yet HTTP GET requests and query param will be put to the test.

Refer to the [complete assignment description][P0] for more details.

[>1]: https://www.repostatus.org "Repo maintenance status"
[>2]: https://choosealicense.com/licenses/gpl-3.0/ "GPL 3.0 License description"

[1]: https://cs50.harvard.edu/web/2020/ "Havard CS50W 2020 course"
[P0]: https://cs50.harvard.edu/web/2020/projects/0/search/ "Project 0: statement"

[B1]: https://www.repostatus.org/badges/latest/concept.svg "Repostatus active badge"
[B2]: https://img.shields.io/github/license/artu-hnrq/havard-cs50w?color=green "License badge"

### Table of Contents
<details>
  <summary>See all</summary>

  * [Getting started](#getting-started)
    * [Development environment](#development-environment)
    * [Continuous automation](#continuos-automation)
  * [Project specifications](#project-specifications)
    * [Folder structure](#folder-structure)
  * [Maintenance](#maintenance-)
  * [License](#license-)

</details>


## Getting started
As a static website, it doesn't take much to get started.
Just access the `index.html` through you preferred browser,
and you'll be ready to go!


### Development environment
You'll still need to have `Git` installed, though:

```bash
$ git --version
git version 2.25.1
```

Thus, clone this repository locally, and you can start developing your project.

### Continuos automation
Project submission is automated through a *submit-on-push* GitHub Action.
It takes in account the branch name to forward the released code to Harvard's `me50/{GITHUB-USERNAME}` repository,
as required.

For it to work you first need to *Authorize cs50*, as specified on *How to Submit* section of project's statements.
Then, register a `PERSONAL_ACCESS_TOKEN` [secret][2] to your repo, as described [here][3]. And you'll be setup!

After that, every push to a branch which name starts with `web50/projects/2020/x/` will be submitted accordingly. 


## Project specifications
*From [project's statement][P0]:* \
**Your website must meet the following requirements:**

- [x] Your website should have at least three pages: one for regular Google Search (which must be called index.html), one for Google Image Search, and one for Google Advanced Search.
  - [x] On the Google Search page, there should be links in the upper-right of the page to go to Image Search or Advanced Search. On each of the other two pages, there should be a link in the upper-right to go back to Google Search.
- [x] On the Google Search page, the user should be able to type in a query, click “Google Search”, and be taken to the Google search results for that page.
  - [x] Like Google’s own, your search bar should be centered with rounded corners. The search button should also be centered, and should be beneath the search bar.
- [x] On the Google Image Search page, the user should be able to type in a query, click a search button, and be taken to the Google Image search results for that page.
- [ ] On the Google Advanced Search page, the user should be able to provide input for the following four fields (taken from Google’s own advanced search options)
  - [ ] Find pages with… “all these words:”
  - [ ] Find pages with… “this exact word or phrase:”
  - [ ] Find pages with… “any of these words:”
  - [ ] Find pages with… “none of these words:”
- [ ] Like Google’s own Advanced Search page, the four options should be stacked vertically, and all of the text fields should be left aligned.
  - [ ] Consistent with Google’s own CSS, the “Advanced Search” button should be blue with white text.
  - [ ] When the “Advanced Search” button is clicked, the user should be taken to the search results page for their given query.
- [ ] Add an “I’m Feeling Lucky” button to the main Google Search page. Consistent with Google’s own behavior, clicking this link should take users directly to the first Google search result for the query, bypassing the normal results page.
  - [ ] You may encounter a redirect notice when using the “I’m Feeling Lucky” button. Not to worry! This is an expected consequence of a security feature implemented by Google.
- [ ] The CSS you write should resemble Google’s own aesthetics.

### Folder structure
For this project, the important files are:
 - `index.html`, which holds the main structure of your website home page
 - `css/style.css`, that contain the website stylesheet entrypoint
 - `js/script.js`, carrying this website logic

```
.
├── .git/                       Version control system folder
├── .github/                    Repo continuous automation 
├── html/                       Website pages
├── css/                        Website stylesheets
├── img/                        Website image directory
├── js/                         Website scripts
├── .gitignore                  VCS ignored files manifest
├── CHANGELOG.md                Release notes description
├── index.html                  Website home page
├── LICENSE                     License file
└── README.md                   Repo readme document
```


## Maintenance [![][B1]][>1]
This project is maintained by the author, [@artu-hnrq](https://github.com/artu-hnrq). \
Though, minimal or no implementation has been done yet,
it's only intended to be a limited example, demo, or proof-of-concept.


## License [![][B2]][>2]
This project is published under the permissions established by [GNU General Public License v3.0][>2].
