# 瀏覽器與網頁原理

- Mozilla 開源專案：Servo
  - 瀏覽器底層核心引擎
  - 平行化瀏覽器
  - Rust 語言寫的 (以前是 C++)
  - GPU WebRender

## 為什麼網頁能在瀏覽器上跑？

瀏覽器會遵照兩個組織實現與修改：

- WHATWG
- W3C

## 他麼差在哪

WHATWG 比較新 (since 2004)，訂定的規範都比較新也比較正確；W3C 比較古老 (since 1994)，常常抄 WHATWG 的規範，還常抄錯。

## 網頁怎麼寫

- HTML
- CSS
- JavaScript
- Image

不會所有資源都收集才秀網頁出來，而是漸進式存取資源

## 瀏覽器架構

- 使用者介面
- 瀏覽器引擎
  - 渲染引擎
  - JS 引擎

## 使用者介面

GUI 應用程式開發框架

- GTK
  - C++，很難寫
- React Native
  - 有前端概念在，比較好寫
- QT

## Search Bar 原理？

- 是否有效 ip or domain name，然後解析它
- 沒有則依據關鍵字查找
- 若有歷史紀錄就會列在下面
- Google 搜尋會有類似 Preview 方式，列在搜尋清單

## 瀏覽器怎麼賺錢？

- 瀏覽器沒有廣告可以賺錢，所以只有兩種賺錢方式
  - 與其他引擎共生關係
  - B2B 方案，有企業客製瀏覽器

## 瀏覽器渲染引擎

- HTML
- CSS

透過 Parse 轉成 Style Tree 與 DOM Tree

### HTML

DOM Tree

### CSS

Rules

```css
Selector {
  declaration
}
```

Style Tree
