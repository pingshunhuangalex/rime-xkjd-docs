---
description: （快捷）符号编码方案
---

# 特殊符号

{% hint style="info" %}
所有键道的符号编码都收录在键道的符号文件中。用户可根据自己的使用习惯随时对其进行修改或拓展（`C:\Users\%USERNAME%\AppData\Roaming\Rime\xkjd6.fuhao.dict.yaml`）
{% endhint %}

## 快捷符号

在日常输入中，标点符号及其组合的使用频率要远远高于其它符号，所以键道收录了常用符号的编码并用`;`键进行引导。下表对这些快捷符号进行了罗列：

| 符号 | 键道编码 | 助记 | 符号 | 键道编码 | 助记 |
| :---: | :---: | :---: | :---: | :---: | :---: |
| ； | `;` | 符号键位 | ‘ | `;n` | `n`、`m`相邻键位 |
| ： | `;;` | 符号键位 | · | `;o` | 符号形似 |
| @ | `;a` | A（t） | —— | `;p` | 破（折号） |
| % | `;b` | 百（分号） | ‰ | `;q` | 千（分号） |
| - | `;c` | `x`、`c`、`v`相邻键位 | ） | `;r` | `e`、`r`相邻键位 |
| 、 | `;d` | 顿（号） | …… | `;s` | 省（略号） |
| （ | `;e` | `e`、`r`相邻键位 | ！ | `;t` | 叹（号） |
| “ | `;f` | `f`、`g`相邻键位 | 《 | `;u` | `u`、`i`相邻键位 |
| ” | `;g` | `f`、`g`相邻键位 | = | `;v` | `x`、`c`、`v`相邻键位 |
| `重复` | `;h` | [H（istory）](extra-functions.md) | ？ | `;w` | 问（号） |
| 》 | `;i` | `u`、`i`相邻键位 | + | `;x` | `x`、`c`、`v`相邻键位 |
| → | `;j` | 箭（头右） | 〇 | `;y` | 圆（圈） |
| ↑ | `;je` | 箭（头）上 | \_\_\_\_ | `;z` | 剩余键位 |
| ↓ | `;jx` | 箭（头）下 | 。” | `;jg` | 符号组合 |
| ← | `;jz` | 箭（头）左 | ……” | `;sg` | 符号组合 |
| 【 | `;k` | `k`、`l`相邻键位 | ！” | `;tg` | 符号组合 |
| 】 | `;l` | `k`、`l`相邻键位 | ？” | `;wg` | 符号组合 |
| ’ | `;m` | `n`、`m`相邻键位 | `次选` | `'` | [编码设计](extra-functions.md) |

{% hint style="info" %}
**笔者私货：**

* 快捷符号的默认键位是从助记的角度出发的，且只考虑了QWERTY的键盘布局。建议根据符号的使用频率、键盘布局与自己的使用习惯重新进行整合分配
* 从上表中可发现符号的次选项未被充分利用，建议用户自行对闲置编码空间进行补充
{% endhint %}

## 带圈符号

键道可以通过输入`o`加上数字的音码部分来快速输入带圈符号。下表对这些带圈符号进行了罗列：

| 带圈符号 | 键道编码 | 带圈符号 | 键道编码 |
| :---: | :---: | :---: | :---: |
| ① | `oyk` | ⑥ | `olq` |
| ② | `oxj` | ⑦ | `oqk` |
| ③ | `osf` | ⑧ | `obs` |
| ④ | `osk` | ⑨ | `ojq` |
| ⑤ | `owj` | ⑩ | `oek` |

## 其它符号

除了快捷符号和带圈符号，键道的符号文件中还存有少量的特殊符号。此处不再赘述。

在此之上，Rime输入平台也内置了海量的符号集可供使用。用户只需输入`/`再加上符号类别便可进行选择（详情可查阅Rime符号文件`C:\Users\%USERNAME%\AppData\Roaming\Rime\symbols.yaml`）。由于符号数量庞大，此处不再一一列举。
