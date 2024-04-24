# Browserbase Documentation

<p align="center" style="max-width: 400px; margin: 0 auto;">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="logo/dark.png"/>
        <img alt="Defer logo" src="logo/light.png"/>
    </picture>
</p>

<p align="center">
    <a href="https://docs.browserbase.com">Documentation</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://www.browserbase.com/">Website</a>
</p>
<br/>

## Introduction

This repository contains the documentation of Browserbase. The documentation is built and deployed using [Mintlify](https://mintlify.com/).

## Quickstart

Install dependencies with:

```bash
npm i -g mintlify
npm install
```


Run the local dev server:

```bash
mintlify dev
```


## Contributing

Before submitting any changes, remember to:

1. Prettify the files:

```bash
npm run prettier
```

2. Check for broken links

```bash
mintlify broken-links
```


### Making changes to the API Reference documentation

Edit the [`api-reference/openapi.json`](api-reference/openapi.json) file and run the following command to generate the MDX files accordingly:

```
npx @mintlify/scraping@latest openapi-file api-reference/openapi.json -o api-reference
```

Then update the [`mint.json`](./mint.json)'s `navigation` part accordingly.