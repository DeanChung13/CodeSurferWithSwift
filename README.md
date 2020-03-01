# Code-Surfer with Swift

[TOC]

## 環境設定

請參考：[Code Surfer](https://github.com/pomber/code-surfer)

```bash
npm init code-surfer-deck my-code
cd my-code
npm start
```



## Swift 語法的支援

Code-Surfer 是透過 `Prism.js` 來解析不同的語言，其中 `Prism`有支援 `Swift`

在 `deck.mdx`的開頭要加入

```
import "prismjs/components/prism-swift"
```

就可以使用

```swift
​```swift
protocol Smaller {
  func smaller() -> Self?
}
​```
```



## Theme

`deck.mdx`的開頭可以加入這些，使用不同的內建主題

```
import { github, nightOwl } from "@code-surfer/themes";
export const theme = nightOwl;

或者

<CodeSurfer theme={nightOwl}>
</CodeSurfer>
```



### Code Surfer 內建的 theme 

`my-deck/node_modules/@code-surfer/themes/dist`

![](https://user-images.githubusercontent.com/1911623/66016573-97df9c00-e4ad-11e9-9095-225d5c9b46a8.png)



### MDX-Deck 內建的 theme

https://github.com/jxnblk/mdx-deck/blob/master/docs/themes.md

```
import { big } from "@mdx-deck/themes";
export const theme = big;
```



# MDX Deck + Code Surfer template

This project was generated with the `npm init code-surfer-deck` command.

## Development

To run the presentation deck in development mode:

```sh
npm start
```

Edit the [`deck.mdx`](deck.mdx) file to get started.

## Exporting

To build the presentation deck:

```sh
npm run build
```

For more documentation see [MDX Deck](https://github.com/jxnblk/mdx-deck) and [Code Surfer](https://codesurfer.pomb.us/)
