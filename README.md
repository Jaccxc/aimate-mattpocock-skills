# Agent Skills

新增了 /ultra-tdd，除此之外 skill 來源皆為 [mattpocock](https://github.com/mattpocock/skills)，可以先去了解他怎麼使用 skills。此 repo 內的下列五個 skills 有針對團隊內版控軟體(gitlab)微調。

## 使用說明

使用前要先安裝 gitlab 專用cli - [glab](https://docs.gitlab.com/cli/) 並先確認可以連接上私有 gitlab

- **使用以下指令安裝五個必要skills**

  ```
  npx skills@latest add Jaccxc/aimate-mattpocock-skills --skill grill-me --skill write-a-prd --skill prd-to-issues --skill tdd --skill ultra-tdd
  ```

## 設計階段 Skill 介紹

- **grill-me** - 設計階段使用，用這個skill幫你分析是不是有些決策或邊際條件你沒想到的
- **write-a-prd** - 用這個skill把你的設計整理成一份 PRD （Product Requirement Document，產品需求文件），也就是把想法寫成一份詳細設計文件，然後自動幫你貼到 Gitlab issue 上
- **prd-to-issues** - 把剛剛貼上去的 PRD 轉成 n 份可以被執行的單元切片，一樣也會重新貼到 Gitlab issue 上

按順序使用以上三個 skill 即可從設計階段走到有多份詳細可執行小計畫的階段

## 開發階段 Skill 介紹

- **tdd** - 把你 gitlab 上的 issue 抓最優先的那一個下來，用 tdd 流程開發

## 特殊開發階段 Skill 介紹 

- **ultra-tdd** - 引入 claude code 最新的 workflow 模式，還有我個人的開發規則，不自己寫程式，而是召喚 agent 去做 /tdd 和各種雜事，節省主 agent 的上下文窗口

ultra-tdd 是我自己根據我平常的流程做的，比較複雜，可以先去看 skill.md 內的內容再決定怎麼套用到你的工作流
