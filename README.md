# 棋盤載入量測

三個頁面功能相同：5×5 空白棋盤，點一格會換色，只差用的技術。要量的是 iPhone 用行動網路第一次打開、到棋盤出現要多久。

build `dbe956c 2026-10-24T05:28Z`

## 怎麼量

1. 關掉 Wi-Fi，只用行動網路。
2. 每一輪開始前，開飛航模式等 3 秒再關掉，等狀態列出現 4G／5G。這樣舊連線會斷掉。
3. 從這一頁依序點下面的連結。**每個連結只點一次**：每個連結都是不同網址，第一次打開一定沒有快取；同一個連結點第二次就會讀到快取。
4. 等頁面上方出現結果，按「複製結果」，回到這一頁點下一個。
5. 全部 9 個點完，把複製的結果一起貼回對話，順便寫是 4G 還是 5G。

**第 1 輪**

- [DOM / SVG](https://9gf6p4448m-del.github.io/board-load-spike/r1/dom/)
- [three.js](https://9gf6p4448m-del.github.io/board-load-spike/r1/three/)
- [Unity WebGL](https://9gf6p4448m-del.github.io/board-load-spike/r1/unity/)

**第 2 輪**

- [three.js](https://9gf6p4448m-del.github.io/board-load-spike/r2/three/)
- [Unity WebGL](https://9gf6p4448m-del.github.io/board-load-spike/r2/unity/)
- [DOM / SVG](https://9gf6p4448m-del.github.io/board-load-spike/r2/dom/)

**第 3 輪**

- [Unity WebGL](https://9gf6p4448m-del.github.io/board-load-spike/r3/unity/)
- [DOM / SVG](https://9gf6p4448m-del.github.io/board-load-spike/r3/dom/)
- [three.js](https://9gf6p4448m-del.github.io/board-load-spike/r3/three/)

