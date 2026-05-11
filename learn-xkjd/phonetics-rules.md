---
description: 音码键位下所蕴含的规则
---

# 键道音码

## 零声母引导

零声母音节是指那些仅由韵母构成的音节（没有辅音声母）。理论上所有以元音`a`、`e`、`i`、`o`、`u`、`ü`开头的音节都是零声母音节，但现代汉语规定`i`、`u`、`ü`开头的音节必须用`w`或`y`进行引导。因此处编码拼合规则键道与传统全拼一致，不再赘述。剩余由`a`、`e`、`o`开头的音节在键道中由零声母`∅`（X键）引导，与传统全拼编码有所不同，故在下表列出：

| 全拼编码  | 键道编码 |
| ----- | ---- |
| `a`   | `xs` |
| `ai`  | `xh` |
| `an`  | `xf` |
| `ang` | `xp` |
| `ao`  | `xz` |
| `e`   | `xe` |
| `ei`  | `xw` |
| `en`  | `xn` |
| `eng` | `xr` |
| `er`  | `xj` |
| `o`   | `xl` |
| `ou`  | `xd` |

## 韵母合并简化

现代汉语中有39个韵母，但键道图谱中却只有33个（M键与X键都有`uang`韵母）。这是因为键道对一&#x4E9B;**“在声韵拼合中没有歧义的”**&#x7EC4;合做了合并简化。

<table><thead><tr><th width="157.22486903371086">键道图谱中的韵母</th><th width="159.33436978152872">现代汉语中的韵母</th><th>合并简化逻辑</th></tr></thead><tbody><tr><td><code>e</code></td><td><code>e</code>、<code>ê</code></td><td><code>ê</code>只在语气词<code>欸</code>中单用，声母均与<code>e</code>拼合，无冲突</td></tr><tr><td><code>i</code></td><td><code>i</code>、<code>-i（前）</code>、<code>-i（后）</code></td><td><code>-i（前）</code>与<code>c</code>、<code>s</code>、<code>z</code>拼合，<code>-i（后）</code>与<code>ch</code>、<code>sh</code>、<code>zh</code>拼合，其余声母均与<code>i</code>拼合，无冲突</td></tr><tr><td><code>uan</code></td><td><code>uan</code>、<code>üan</code></td><td><code>üan</code>与<code>j</code>、<code>q</code>、<code>x</code>、<code>y</code>拼合，其余声母均与<code>uan</code>拼合，无冲突</td></tr><tr><td><code>eng</code></td><td><code>eng</code>、<code>ueng</code>、<code>ng</code></td><td><code>ueng</code>只是一种<code>weng</code>的零声母音节形式，实际使用中声母均与<code>eng</code>拼合，无冲突<br><br><code>ng</code>只在语气词中使用，和与<code>eng</code>拼合的声母均无冲突</td></tr><tr><td><code>un</code></td><td><code>un</code>、<code>ün</code></td><td><code>ün</code>与<code>j</code>、<code>q</code>、<code>x</code>、<code>y</code>拼合，其余声母均与<code>un</code>拼合，无冲突</td></tr></tbody></table>

## j、q、x、y声韵拼合

从上述韵母合并简化逻辑中不难看出，键道的键位设计脱胎于声韵拼合规则，而不是将书写后的拼音映射到不同键位上。由于不涉及`ü`韵母省写规则，键道编码在处理特定的`j`、`q`、`x`、`y`声韵拼合时与传统全拼编码有所不同，故在下表中列出：

| 全拼编码      | 键道编码 |
| --------- | ---- |
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

<table><thead><tr><th width="150">声母</th><th width="170">声母键位</th><th>可拼合韵母</th></tr></thead><tbody><tr><td><code>ch</code></td><td>仅J键（外侧）</td><td><code>ai</code>、<code>an</code>、<code>ang</code>、<code>en</code>、<code>eng</code>、<code>u</code>、<code>un</code></td></tr><tr><td><code>ch</code></td><td>仅W键（内侧）</td><td><code>a</code>、<code>i</code>、<code>ong</code>、<code>ou</code>、<code>ua</code>、<code>uai</code>、<code>uan</code>、<code>uang</code>、<code>ui</code>、<code>uo</code></td></tr><tr><td><code>ch</code></td><td>J键、W键（<a href="../advance-in-xkjd/alt-code.md">飞键</a>）</td><td><code>ao</code>、<code>e</code></td></tr><tr><td><code>zh</code></td><td>仅Q键（外侧）</td><td><code>an</code>、<code>ang</code>、<code>ei</code>、<code>en</code>、<code>eng</code>、<code>u</code>、<code>un</code></td></tr><tr><td><code>zh</code></td><td>仅F键（内侧）</td><td><code>a</code>、<code>i</code>、<code>ong</code>、<code>ou</code>、<code>ua</code>、<code>uai</code>、<code>uan</code>、<code>uang</code>、<code>ui</code>、<code>uo</code></td></tr><tr><td><code>zh</code></td><td>Q键、F键（<a href="../advance-in-xkjd/alt-code.md">飞键</a>）</td><td><code>ai</code>、<code>ao</code>、<code>e</code></td></tr></tbody></table>
