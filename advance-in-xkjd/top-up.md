---
description: 词词相扣，音形灵动
---

# 顶功（上屏）

{% hint style="info" %}
与[简码](shorthand.md)类似，是否熟悉与掌握顶功并不影响键道的日常使用，但是其对输入效率的提升起着决定性的作用。顶功在键道的使用中随处可见，因此理解记忆下列需要使用空格键（`␣`）分隔上屏的情况其实更为简便：

* 上屏除特殊简码外的所有简码首选（一级、二级、三级简码）
* 上屏无需形码（辅助码）的单字首选（声 + 韵）
* 上屏无需形码（辅助码）的三字词组首选（声 + 声 + 声）
* 上屏形码键所对应的一级简码之前的任何字词
{% endhint %}

顶功是指在输入过程中，由输入方案根据编码结构推断字词的编码尾部，从而自动上屏已确认的编码部分。得益于键道音码形码完全分离的设计，用户在大多数情况下不需要刻意使用空格键（`␣`）对输入中的编码进行分隔确认。这种设计在显著减少空格键（`␣`）击打的同时，也大大提升了输入效率与手感。

## 键道上屏技巧

### 顶功上屏

顶功的本质在于无损耗地（无需确认键）通过后续的输入将前一字词顶上屏幕。在上屏时如有多个候选项，则默认上屏首选项。由于键道字词都是先输入音码定音再输入形码选重（不包括形码键所对应的一级简码），所以在任意形码后输入音码都会使音码之前的编码自动上屏。

### 定长上屏

定长上屏是指在输入过程中，当达到最大码长时自动上屏已输入的编码部分。根据[词组](../start-xkjd/phrases.md)章节，键道词组的音码部分码长最高只有4位。所以当连续输入5个音码时，编码的前四位将会自动上屏，并保留第五个编码等待后续输入（无需确认键）。

类似于音码的码长限制，根据[单字](../start-xkjd/characters.md)与[词组](../start-xkjd/phrases.md)章节，键道字词的总码长最高只有6位。所以当连续输入7个编码时，编码的前六位将会自动上屏，并保留第七个编码等待后续输入（无需确认键）。

## 其它上屏技巧

### 空格上屏

空格上屏是输入法中最常见的上屏方式。在传统输入法中空格键（`␣`）担任着确认键的角色。几乎所有字、词、短语、句子都依靠空格键（`␣`）进行分隔并上屏。在键道中除开个别编码有歧义的情况外（见上方总结），用户无需使用空格键（`␣`）对输入中的编码进行分隔上屏。

{% hint style="warning" %}
严格意义上来说，空格上屏的候选项并非首选项，而是**“处于焦点停留状态的”**候选项（默认的焦点停留位置为首选项）。用户可使用上/下方向键或翻页键移动焦点并使用空格键（`␣`）上屏相应的候选项（不推荐）
{% endhint %}

### 选重上屏（数字）

和传统输入法相同，键道也可以通过数字键进行选重上屏（不推荐）。与空格上屏相似，选重上屏（数字）也是一种选择上屏，即通过牺牲数字键本来的作用来上屏对应序列号的候选项。

### 选择上屏

选择上屏是指用特定的按键来上屏相应位置的候选项。其特点在于在上屏过程中，选择键失去了原来的作用而仅执行选择这一功能，是一种有损耗的上屏方式。从本质上来说，空格、次选键（`'`）与数字键上屏都属于选择上屏，即通过牺牲按键本来的作用来上屏特定的候选项（次选键介绍可参考[特殊功能](../master-xkjd/extra-functions.md)章节）。

### 非码上屏（符号）

非码上屏是指在输入过程中，当输入的字符不参与编码时自动上屏已输入的编码部分。在键道中非编码字符一般指各种（标点）符号。需要注意的是，用于上屏的键位本身不能有其它功能，比如移动焦点或翻页用的字符是无法同时执行上屏操作的。熟悉与掌握非码上屏能在符号出现的场景中节省一个确认键位。

### 唯一上屏

唯一上屏是指在编码唯一且追加任何编码字符都是空码时自动上屏已输入的编码部分。这个特性和键道的词库优化息息相关（废词占码越多，上屏效率越差），一般无需刻意进行掌握。

{% hint style="warning" %}
需要注意的是，唯一上屏的触发需要同时满足**“编码唯一”**与**“追加任何编码字符都是空码”**这两个条件。在输入过程中有时会出现候选项只剩一个但仍没有自动上屏的情况，这是因为词库中该字词保留了其全码形式。此时使用顶功或空格键（`␣`）进行分隔可提前上屏该字词
{% endhint %}

### 空码上屏

空码上屏是指在输入过程中，如果输入的字符与已输入的编码部分构成了空码，则将已输入的编码部分自动上屏，同时留下导致空码的字符等待后续输入（无需确认键）。从本质上来说，顶功上屏、定长上屏、非码上屏（符号）和唯一上屏都是空码上屏的应用。而键道就是通过独特的编码设计使输入过程中自然地出现空码上屏从而提升输入效率与手感。
