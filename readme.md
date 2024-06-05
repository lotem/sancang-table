# 三碼蒼頡碼表

利用蒼六碼表和 IDS數據庫生成三碼倉頡碼表。

成品碼表用於 Rime 輸入方案 [三碼蒼頡](https://github.com/lotem/rime-sancang)

做法：

  - 將 [齋版 Cangjie6 碼表][1] 和 [IDS 數據庫][2] 關聯起來，得到 `decomp.tsv`；
  - 參照 IDS 字形解構信息，檢索並在構詞碼中用 `/` 標記出蒼六反字身字的字首、字身；
  - 並利用構詞碼中的包含結構標記 `'` 通過模式匹配生成三蒼碼表 `sancang.tsv`。

[1]: https://github.com/LEOYoon-Tsaw/Cangjie6
[2]: https://github.com/cjkvi/cjkvi-ids
