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
