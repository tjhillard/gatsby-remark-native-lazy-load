# gatsby-remark-native-lazy-load

Adds [native lazy loading](https://addyosmani.com/blog/lazy-loading/) to your markdown images.

Input
```md
![Foo](https://i.imgur.com/dc1PU8j.jpg)
```

Output
```html
<img src="https://i.imgur.com/dc1PU8j.jpg" alt="Foo" loading="lazy">
```

## Install

```bash
yarn add gatsby-remark-native-lazy-load
```

```bash
npm i gatsby-remark-native-lazy-load --save
```

## Usage

```js
{
  resolve: `gatsby-transformer-remark`,
  options: {
    plugins: [
      `gatsby-remark-native-lazy-load`,
    ],
  },
}
```