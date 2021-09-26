---
description: 音码键位下所蕴含的规则
---

# 键道音码

## 零声母引导

零声母音节是指那些仅由韵母构成的音节（没有辅音声母）。理论上所有以元音`a`、`e`、`i`、`o`、`u`、`ü`开头的音节都是零声母音节，但现代汉语规定`i`、`u`、`ü`开头的音节必须用`w`或`y`进行引导。因此处编码拼合规则键道与传统全拼一致，不再赘述。剩余由`a`、`e`、`o`开头的音节在键道中由零声母`∅`（X键）引导，与传统全拼编码有所不同，故在下表列出：

| 全拼编码 | 键道编码 |
| :--- | :--- |
| `a` | `xs` |
| `ai` | `xh` |
| `an` | `xf` |
| `ang` | `xp` |
| `ao` | `xz` |
| `e` | `xe` |
| `ei` | `xw` |
| `en` | `xn` |
| `eng` | `xr` |
| `er` | `xj` |
| `o` | `xl` |
| `ou` | `xd` |

## 韵母合并简化

现代汉语中有39个韵母，但键道图谱中却只有33个（M键与X键都有`uang`韵母）。这是因为键道对一些**“在声韵拼合中没有歧义的”**组合做了合并简化。

| 键道图谱中的韵母 | 现代汉语中的韵母 | 合并简化逻辑 |
| :--- | :--- | :--- |
| `e` | `e`、`ê` | `ê`只在语气词`欸`中单用，声母均与`e`拼合，无冲突 |
| `i` | `i`、`-i（前）`、`-i（后）` | `-i（前）`与`c`、`s`、`z`拼合，`-i（后）`与`ch`、`sh`、`zh`拼合，其余声母均与`i`拼合，无冲突 |
| `uan` | `uan`、`üan` | `üan`与`j`、`q`、`x`、`y`拼合，其余声母均与`uan`拼合，无冲突 |
| `eng` | `eng`、`ueng` | `ueng`只是一种`weng`的零声母音节形式，实际使用中声母均与`eng`拼合，无冲突 |
| `un` | `un`、`ün` | `ün`与`j`、`q`、`x`、`y`拼合，其余声母均与`un`拼合，无冲突 |

## j、q、x、y声韵拼合

从上述韵母合并简化逻辑中不难看出，键道的键位设计脱胎于声韵拼合规则，而不是将书写后的拼音映射到不同键位上。由于不涉及`ü`韵母省写规则，键道编码在处理特定的`j`、`q`、`x`、`y`声韵拼合时与传统全拼编码有所不同，故在下表中列出：

| 全拼编码 | 键道编码 |
| :--- | :--- |
| `ju`/`jv` | `jl` |
| `qu`/`qv` | `ql` |
| `xu`/`xv` | `xl` |
| `yu`/`yv` | `yl` |

## ch、zh音节避重

观察键道图谱可发现，有两个翘舌声母（`ch`、`zh`）和一个韵母（`uang`）都各出现了两次。其中韵母`uang`（M键、X键）可与任意声母进行拼合（详情可参考[飞键](../advance-in-xkjd/alt-code.md)章节），而声母`ch`（J键、W键）和`zh` （F键、Q键）在与韵母拼合时却需要遵循某些规则。该设计的初衷是在声韵键位分布与击键手感间达到一种平衡，同时也是一种妥协。

{% hint style="info" %}
在标准图谱中，将两个翘舌声母（`ch`、`zh`）所在的键位排成一排可得`Q`、`W`、`F`、`J`。其中外侧的`ch`、`zh`声母（J键、Q键）与`a`、`e`开头的韵母（不含`a`、`e`韵母本身）**所在键位的韵母**进行拼合，而内侧的`ch`、`zh`声母（W键、F键）与**其余键位的韵母**进行拼合
{% endhint %}

以上规则在理解后可起到助记作用，但规则本身过于晦涩拗口。为帮助初学者进行理解，下表对所有相关的声韵组合进行了罗列：

| 声母 | 声母键位 | 可拼合韵母 |
| :--- | :--- | :--- |
| `ch` | 仅J键（外侧） | `ai`、`an`、`ang`、`ao`、`en`、`eng`、`u`、`un` |
| `ch` | 仅W键（内侧） | `a`、`i`、`ong`、`ou`、`uan`、`uang`、`ui`、`uo` |
| `ch` | J键、W键（[飞键](../advance-in-xkjd/alt-code.md)） | `ao`、`e` |
| `zh` | 仅Q键（外侧） | `an`、`ang`、`en`、`eng`、`u`、`un` |
| `zh` | 仅F键（内侧） | `a`、`i`、`ong`、`ou`、`ua`、`uai`、`uan`、`uang`、`ui`、`uo` |
| `zh` | Q键、F键（[飞键](../advance-in-xkjd/alt-code.md)） | `ai`、`ao`、`e` |
