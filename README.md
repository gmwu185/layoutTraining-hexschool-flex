## 頁面連結
- [flex grid](https://gmwu185.github.io/layoutTraining-hexschool-flex/flexGrid.html)
- [主要頁面](https://gmwu185.github.io/layoutTraining-hexschool-flex/index.html)



## gulp 套件與版本說明
- gulp 4 自動化執行前端檔案編譯與產出

### 安裝環境

需先安裝 Node。

```
npm install gulp -g
```

### 執行

請依序執行以下指令來執行 gulp。

```
npm install
gulp
```


## 工具類與 flex grid 格線系統，透過 Scss 量產與應用設計

- 自製 flex grid 格線系統，簡單的斷點設計讓版面自適應 (RWD)，另外利用 ``flex: flex-grow | flex-shrink | flex-basis`` 屬性設計更高彈性的等分規劃，配合計算公式讓排版更加精準與靈活。
- 透過 Scss for if 製作批次格線系統與空間工具樣式，單純修改變數可達到更多與精細的設定 (會有肥大問題，但以受用範圍為主，少量就獨立出來)，另外增加複用性。
- 使用 flex grid 格線系統替換區塊語意式 class 樣式命名，將 HTML tag 為主增加可視性 (不會都是一路 div)。



## CSS 命名字符組設定 
- 前綴 ``c`` 元件類、``p`` 特頁用類、``l`` 共用與全站類、``u`` 工具類
- ``-`` 關連性 (口語化可視為的)
- ``__`` BEM 元素或下層
- ``--`` BEM 修飾子，另外結合參數數值的應用以延伸性為主，如果沒帶上為基本設定。

### 以 flxeGrid 格線系統命名字符使用說明

``.l-fg-col--12-1 ``：``l`` 前綴、``fg`` flxeGrid 縮寫、``col`` 欄寬、``--`` 後接的是等分數。
整個較口語化可記得為：共用類型的 flex 格線系統的欄寬等分為 12 分之 1 (12 等分的 1 份)。