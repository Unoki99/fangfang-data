# 方方詞卡：詞典的原始檔案

[方方詞卡](https://github.com/unoki99/fangfang-cards)（App、瀏覽器的查詞外掛和安裝程式）安裝詞典時先從這裡下載，這裡下載不到時才從原本發布的地方下載。這些檔案不在方方詞卡的 MIT 授權範圍內。
這裡的檔案都**和原本發布的一模一樣，沒有任何修改**（下載日期：2026-11-20），只有 `common/wiktionary-zh-*.jsonl.gz` 例外（見最下面）。每個檔案依照它自己的授權。

| 資料夾／檔案 | 來源 | 授權 |
|---|---|---|
| `tw/kautian.ods` | 教育部《臺灣台語常用詞辭典》 https://sutian.moe.edu.tw/ | [CC BY-ND 3.0 臺灣](https://creativecommons.org/licenses/by-nd/3.0/tw/) |
| `hak/*腔詞條詞目文字.ods` | 教育部《臺灣客語辭典》 https://hakkadict.moe.edu.tw/ | [CC BY-ND 3.0 臺灣](https://creativecommons.org/licenses/by-nd/3.0/tw/) |
| `zh/dict-revised.json.xz` | 教育部《重編國語辭典修訂本》，g0v 萌典整理 https://github.com/g0v/moedict-data | [CC BY-ND 3.0 臺灣](https://creativecommons.org/licenses/by-nd/3.0/tw/) |
| `zh/dict-csld.json` | 中華文化總會《兩岸常用詞典》，g0v 萌典整理 https://github.com/g0v/moedict-data-csld | [CC BY-NC-ND 3.0 臺灣](https://creativecommons.org/licenses/by-nc-nd/3.0/tw/)（非商業） |
| `zh/hsk30.csv`、`zh/hsk30-chars.csv` | HSK 3.0 詞表 https://github.com/ivankra/hsk30 | MIT（見 `zh/hsk30-LICENSE.txt`） |
| `zh/ids.txt` | cjkvi-ids https://github.com/cjkvi/cjkvi-ids （源自 CHISE 計畫） | 依 CHISE 的授權（GPL，見 `common/GPL-2.0.txt`） |
| `zh/cj.yaml`、`zh/cjx.yaml` | Rime 倉頡五代 https://github.com/rime/rime-cangjie | LGPL-3.0（見 `common/LGPL-3.0.txt`、`common/GPL-3.0.txt`） |
| `zh/wb.yaml` | Rime 五筆 86 https://github.com/rime/rime-wubi | LGPL-3.0（見 `common/LGPL-3.0.txt`、`common/GPL-3.0.txt`） |
| `common/essay.txt` | rime-essay 詞頻 https://github.com/rime/rime-essay | LGPL-3.0（見 `common/LGPL-3.0.txt`、`common/GPL-3.0.txt`） |
| `common/cedict_ts.u8` | CC-CEDICT https://cc-cedict.org/ | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| `yue/CC-CANTO.txt`、`yue/READINGS.txt` | CC-Canto（Pleco），經 jyut-dict https://github.com/aaronhktan/jyut-dict | [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) |
| `yue/jyut6ping3.*.dict.yaml`、`yue/essay-cantonese.txt` | rime-cantonese https://github.com/rime/rime-cantonese | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| `yue/yyzd.txt` | 開放粵語字典（© 2009–2020 開放詞典 kaifangcidian.com） https://github.com/kfcd/yyzd | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)（見 `yue/yyzd-LICENSE.txt`） |
| `ja/JMdict_e_examp.gz`、`ja/kanjidic2.xml.gz` | JMdict、KANJIDIC2（EDRDG） https://www.edrdg.org/ | [CC BY-SA 4.0](https://www.edrdg.org/edrdg/licence.html) |
| `sv/folkets.xml` | Folkets lexikon（KTH） http://folkets-lexikon.csc.kth.se/folkets/ | [CC BY-SA 2.5](https://creativecommons.org/licenses/by-sa/2.5/) |
| `sv/sv_50k.txt` | FrequencyWords（Hermit Dave） https://github.com/hermitdave/FrequencyWords | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| `sv/zhwikt-sv.jsonl` | 中文維基詞典的瑞典語詞，kaikki.org 整理 https://kaikki.org/ | [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) |
| `common/wiktionary-zh-*.jsonl.gz`（`common/wiktionary-zh.txt` 列出全部） | 英文維基詞典的中文詞，kaikki.org（wiktextract）整理 https://kaikki.org/dictionary/Chinese/ **（有修改：只留下 App 用到的部分，見下面）** | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |
| `sw/swjz.xml` | 段玉裁《說文解字注》，cjkvi-dict https://github.com/cjkvi/cjkvi-dict | [GPLv2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html)（見 `common/GPL-2.0.txt`） |

不包含 TOCFL 詞表（沒有授權，不能轉載）：App 仍然從 https://github.com/ivankra/tocfl 下載。

## `common/wiktionary-zh-*.jsonl.gz` 的修改

這是唯一不是原樣的檔案。原本的 kaikki.org-dictionary-Chinese.jsonl（英文維基詞典的中文詞，kaikki.org 用 wiktextract 整理，
CC BY-SA 4.0）有 1.1 GB，GitHub 放不下，kaikki.org 也說之後會拿掉。這裡只留下方方詞卡用到的：每個中文詞的寫法、詞性、
讀音（zh_pron、粵語錄音的網址）、意思（glosses 和標籤）、粵拼例句、各地說法（synonyms）；其他的（翻譯、詞源、其他的讀音
標記等等）拿掉了，再壓縮成不到 90 MB 的幾個檔案。內容來自維基詞典的作者們（https://en.wiktionary.org/ ），依 CC BY-SA 4.0
分享，這些檔案也是同樣的授權。製作日期：2026-11-20。
