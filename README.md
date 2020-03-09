# react-native-docs

facebook/[react-native-website](https://github.com/facebook/react-native-website):https://reactnative.dev  
[Docusaurus](https://docusaurus.io/en/) · Easy to Maintain Open Source Documentation

Run the Docusaurus installation script: `npx docusaurus-init`
The Docusaurus installation script will create two new directories: `docs` and `website`

Running the example website

`$ cd website`  
`$ yarn start`  
 http://localhost:3000

## Publish the Site

[tutorial-publish-site](https://docusaurus.io/docs/zh-CN/tutorial-publish-site)  
Edit the file `docusaurus-tutorial/website/siteConfig.js`

website\siteConfig.js

```js
const siteConfig = {
  title: 'Test Site', // Title for your website.
  tagline: 'A website for testing',
  url: 'https://jacobhsu.github.io', // Your website URL
  baseUrl: '/react-native-docs/', // Base URL for your project */

  // Used for publishing and more
  projectName: 'react-native-docs',
  organizationName: 'jacobhsu',
```

`$ GIT_USER=jacobhsu CURRENT_BRANCH=master USE_SSH=true yarn run publish-gh-pages`  
`$ yarn b`  
`$ yarn d`  

## pre code

```js
  highlight: {
    // default, Highlight.js theme to use for syntax highlighting in code blocks.
    theme: 'solarized-dark',
  },
```

website\static\css\syntax.css

## debug

Error: Processing the following `doc` field in `headerLinks` within `siteConfig.js`: 'gettin
g-started' It looks like there is no document with that id that exists in your docs director
y. Please double check the spelling of your `doc` field and the `id` fields of your docs.
 
```js
---
id: getting-started #fixed
title: Getting Started
original_id: getting-started
---
```

website\versioned_docs\version-0.61\getting-started.md

```js
---
id: version-0.61-getting-started
title: Getting Started
original_id: getting-started
---
```
