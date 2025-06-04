<div align="center">

[![DocSearch](.github/logo.svg)](https://docsearch.algolia.com)

The easiest way to add search to your documentation – for free.

[![Netlify Status](https://api.netlify.com/api/v1/badges/30eacc09-d4b2-4a53-879b-04d40aaea454/deploy-status)](https://app.netlify.com/sites/docsearch/deploys) [![npm version](https://img.shields.io/npm/v/@docsearch/js.svg?style=flat-square)](https://www.npmjs.com/package/@docsearch/js/v/alpha) [![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)](./LICENSE)

<p align="center">
  <strong>
  <a href="https://docsearch.algolia.com">Documentation</a> •
  <a href="https://codesandbox.io/s/docsearchjs-v3-playground-z9oxj">JavaScript Playground</a> •
  <a href="https://codesandbox.io/s/docsearch-react-v3-playground-619yg">React Playground</a>
  </strong>
</p>

</div>

---

DocSearch crawls your documentation, pushes the content to an Algolia index and provides a dropdown search experience on your website.

## Preview

![Screencast](.github/screencast.gif)

| Light | Dark |
| --- | --- |
| ![Light preview](.github/preview-light.png) | ![Dark preview](.github/preview-dark.png) |

## Usage

> Don't have your Algolia credentials yet? [Apply to DocSearch](https://docsearch.algolia.com/apply)!

### JavaScript

#### Installation

```sh
yarn add @docsearch/js@3
# or
npm install @docsearch/js@3
```

If you don’t want to use a package manager, you can use a standalone endpoint:

```html
<script src="https://cdn.jsdelivr.net/npm/@docsearch/js@3"></script>
```

#### Get started

To get started, you need a [`container`](https://docsearch.algolia.com/docs/api#container) for your DocSearch component to go in. If you don’t have one already, you can insert one into your markup:

```html
<div id="docsearch"></div>
```

Then, insert DocSearch into it by calling the [`docsearch`](https://docsearch.algolia.com/docs/api) function and providing the container. It can be a [CSS selector](https://developer.mozilla.org/en-us/docs/web/css/css_selectors) or an [Element](https://developer.mozilla.org/en-us/docs/web/api/htmlelement).

Make sure to provide a [`container`](https://docsearch.algolia.com/docs/api#container) (for example, a `div`), not an `input`. DocSearch generates a fully accessible search box for you.

```js app.js
import docsearch from '@docsearch/js';

import '@docsearch/css';

docsearch({
  container: '#docsearch',
  appId: 'YOUR_APP_ID',
  indexName: 'YOUR_INDEX_NAME',
  apiKey: 'YOUR_SEARCH_API_KEY',
});
```

### React

#### Installation

```bash
yarn add @docsearch/react@3
# or
npm install @docsearch/react@3
```

If you don’t want to use a package manager, you can use a standalone endpoint:

```html
<script src="https://cdn.jsdelivr.net/npm/@docsearch/react@3"></script>
```

#### Get started

DocSearch generates a fully accessible search box for you.

```jsx App.js
import { DocSearch } from '@docsearch/react';

import '@docsearch/css';

function App() {
  return (
    <DocSearch
      appId="YOUR_APP_ID"
      indexName="YOUR_INDEX_NAME"
      apiKey="YOUR_SEARCH_API_KEY"
    />
  );
}

export default App;
```

## Styling

[Read documentation →](https://docsearch.algolia.com/docs/styling)

## Related projects

DocSearch is made of the following repositories:

- **[algolia/docsearch](https://github.com/algolia/docsearch)**: DocSearch source code.
- **[algolia/docsearch/packages/website](https://github.com/algolia/docsearch/tree/main/packages/website)**: DocSearch website and documentation.
- **[algolia/docsearch-configs](https://github.com/algolia/docsearch-configs)**: DocSearch websites configurations that DocSearch powers.
- **[algolia/docsearch-scraper](https://github.com/algolia/docsearch-scraper)**: DocSearch crawler that extracts data from your documentation.

## License

[MIT](LICENSE)

-----------------

Save 100s of hours of work by using Page AI to generate a beautiful website. In just minutes!

| | |
| :- | :- |
| <a href="https://pageai.pro" target="_blank"><img height="60px" src="https://pageai.pro/static/images/logo-square.png" alt="Page AI Logo" /></a> <br/> <b>Page AI</b> <br/> AI Website Generator that designs and writes clean code. <br/><br/> Try the app on <a href="https://pageai.pro">pageai.pro</a>. | <a href="https://pageai.pro" target="_blank"><img width="300px" src="https://user-images.githubusercontent.com/1515742/281077548-57b24773-3c2a-4e89-b088-cc3945d7037b.png" alt="Page AI Logo" /></a> |

-----------------

Apihustle is a collection of tools to test, improve and get to know your API inside and out. <br/>
[apihustle.com](https://apihustle.com) <br/>

|                                                                                                                                                                                        |              |                                                          |                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------- | :------------------------------------------------------- | :------------------------------------------- |
| <a href="https://pageai.pro" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/9bfbfe6f-add9-45de-aaf2-5c6043a47e41" alt="Page AI Logo" /></a>        | **Page AI**  | AI Website Generator that designs and writes clean code. | [pageai.pro](https://pageai.pro)             |
| <a href="https://shipixen.com" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/e1deba72-328e-4d3c-9c62-11ab77184561" alt="Shipixen Logo" /></a>     | **Shipixen** | Create a personalized blog & landing page in minutes     | [shipixen.com](https://shipixen.com)         |
| <a href="https://pageui.dev" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/b8815b62-598a-4fca-bc27-c03e66c8b105" alt="Page UI Logo" /></a>        | **Page UI**  | Landing page UI components for React & Next.js           | [pageui.dev](https://pageui.dev)             |
| <a href="https://clobbr.app" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/cb3e64e2-efaa-436b-ae6d-0ea4b47e4004" alt="Clobbr Logo" /></a>         | **Clobbr**   | Load test your API endpoints.                            | [clobbr.app](https://clobbr.app)             |
| <a href="https://crontap.com" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/38a3d734-d1ca-4f92-9cfb-ada52b9f2ffb" alt="Crontap Logo" /></a>       | **Crontap**  | Schedule API calls using cron syntax.                    | [crontap.com](https://crontap.com)           |
| <a href="https://tool.crontap.com" target="_blank"><img  width="54px" src="https://github.com/user-attachments/assets/545f7618-ff2c-47fa-ad17-e17e38155f55" alt="CronTool Logo" /></a> | **CronTool** | Debug multiple cron expressions on a calendar.           | [tool.crontap.com](https://tool.crontap.com) |

-----------------

<a href="https://apihustle.com" target="_blank">
  <img height="60px" src="https://user-images.githubusercontent.com/1515742/215217833-c07183d2-f688-4d1c-86ea-329f3b28f81c.svg" alt="Apihustle Logo" />
</a>

-----------------
