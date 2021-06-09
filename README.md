<p align="center"><a href="https://www.glue.codes" target="_blank" rel="noopener noreferrer"><img width="100" src="https://github.com/gluecodes/gluecodes-widgets/blob/master/mediaFiles/logo.png" alt="GlueCodes Studio"></a></p>

<h1 align="center">@gluecodes/global-styles</h1>

This repo contains Global Styles to be used within [GlueCodes Studio](https://www.glue.codes) by a single-click insertion.

## Table of contents
- [Setup](#setup)
  - [Preparing GlueCodes Studio](#preparing-glueCodes-studio)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Git flow](#git-flow)
  - [Your first Global Styles](#your-first-global-styles)
  - [Anatomy of a Global Styles](#anatomy-of-global-styles)
- [Styling rules](#styling-rules)
- [Before shipping](#before-shipping)
- [Using this repo in GlueCodes Studio](#using-this-repo-in-glueCodes-studio)
- [License](#license)
- [Subscribe](#subscribe)

## Setup

### Preparing GlueCodes Studio

- Go to [GlueCodes](https://www.glue.codes) website and navigate to GlueCodes Studio. Before you get access to the project manager you might be asked to login via GitHub or Google. Please note that the Studio is NOT asking for any permissions to your GitHub repositories or personal data.
- In the project manager you can navigate to the tab [Demos](https://ide.glue.codes/?openedTab=demos) where you can find templates with pre-installed Widgets and the Global Style file with all classes.
- Remember that you don't need to style every single class to submit your work.

### Prerequisites

- Terminal (on Windows you may use PowerShell).
- You must have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed.

### Installation

In your terminal, run the commands below:

- Clone this repo: `git clone git@github.com:gluecodes/gluecodes-global-styles.git` or `git clone https://github.com/gluecodes/gluecodes-global-styles.git`.

### Git flow

We use a custom Git flow which is based on the feature branches. Before you jump into styling, name your branch according to these rules:

- When developing a new Global Styles: `git checkout -b feature/someGlobalStylesName`.

Always create your branch off master. When you're ready, just create a pull request. Remember to rebase onto `master` before requesting a code review in your pull request (`git rebase origin/master -i` and follow the instructions). You'll find more details in a pull request description template.

### Your first Global Styles

- Go to: `src/ui/` and duplicate example directory and name it with your intended Global Styles name.

### Anatomy of a Global Styles

A Global Styles are made out of the following files:

```
.
|-- googleFonts.json            <-- Google fonts to be imported, they will be preloaded at the app level
|-- readme.js                   <-- a function returning brief description, author and tags of the Global styles which are visible in GlueCodes Studio
|-- styles.css                  <-- styles that will be availaible in GlueCodes Studio
|-- thumbnail.jpg               <-- a image representing your Global STyles. It will be visible in GlueCodes Studio.
```

## Styling rules

Here is a few rules to follow when styling your components:

- Choose clean and good looking design over fulfilling all the classes.
- The `styles.css` should contain style declarations with class selectors.
- Don't rely on external libraries, use pure CSS.
- Use media queries and breakpoints recommended by [Bootstrap](https://getbootstrap.com/docs/4.0/layout/overview/).
- Add the Google Fonts you want to import into `googleFonts.json`. [Read more](https://github.com/gluecodes/gluecodes-widgets/blob/master/googleFonts.md) about importing fonts and taking advantage of font preloading.

### Before shipping

Remember to document your Global Styles before requesting a code review. Fill in `./readme.js`. Also don't forget about a relevant  `./thumbnail.jpg`.

Here is an example of `./brief.json`:

```json
{
  "author": "Your name",
  "description": "short description",
  "tags": [
    "modern"
  ]
}
```

## Using this repo in GlueCodes Studio

To insert Global Style sheet in GlueCodes Studio you simply need to navigate to Global Styles file where you get access to library connected to this repo. After you click 'insert' the CSS will be inserted into the file that you are on. 

## License

[MIT](https://github.com/gluecodes/gluecodes-widgets/blob/master/LICENSE)

## Subscribe

Subscribe to our social media channels for tutorials and latest news.

- [YouTube](https://www.youtube.com/channel/UCDtO8rCRAYyzM6pRXy39__A)
- [Facebook](https://www.facebook.com/groups/gluecodesstudio)
- [LinkedIn](https://www.linkedin.com/company/gluecodes)