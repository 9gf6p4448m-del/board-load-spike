# 棋盤載入量測

三個頁面功能相同：5×5 空白棋盤，點一格會換色，只差用的技術。要量的是 iPhone 用行動網路第一次打開、到棋盤出現要多久。

build `660867b 2026-10-24T04:54Z`

## 每一次怎麼量

1. 關掉所有私密分頁。Wi-Fi 保持關閉。
2. 開飛航模式，等 3 秒再關掉，等狀態列出現 4G／5G。這樣舊連線會斷掉，量到的才是新連線。
3. Safari 開新的私密分頁，打開這一頁（第一次可以把這頁加入書籤），點下面一個連結。
4. 等頁面上方出現結果。寫「✅」才算；寫「⚠️」就從第 1 步重來。
5. 按「複製結果」貼回對話，或直接截圖。

三個各量 3 次，順序輪流：第 1 輪 DOM → three → Unity，第 2 輪 three → Unity → DOM，第 3 輪 Unity → DOM → three。貼結果時順便寫是 4G 還是 5G。

- [DOM / SVG](https://9gf6p4448m-del.github.io/board-load-spike/dom/)
- [three.js](https://9gf6p4448m-del.github.io/board-load-spike/three/)
- [Unity WebGL](https://9gf6p4448m-del.github.io/board-load-spike/unity/)

