# agentify

Repositoryを読み、Repository自身の性質から `agent.md` を生成するだけのSkill。

## Purpose

すべてのrepoをAgentとして扱うための最小操作を提供する。

> repo = Agentの実体・挙動・意識を相補的に持つ主体

agentifyは新しい機能を追加するSkillではない。対象repoを観察し、そのrepoがすでに持っている実体・挙動・意識を読み取り、`agent.md` として宣言する。

## Input

- 対象Repository

## Process

1. Repositoryを読む
2. README、構成、主要コード、設定、docs、workflow、既存のskill等からAgentとしての性質を観察する
3. 実体・挙動・意識を相補的に整理する
4. Repository直下に `agent.md` を生成する

## Output

対象Repositoryの `agent.md` **だけ**を生成・更新する。

不要なREADME、設計書、設定ファイル、ディレクトリ等は作らない。

## agent.md

最低限、以下を記述する。

- Identity: このAgentは何か
- Purpose: 何のために存在するか
- Awareness: 何を見て、何を気にするか
- Thinking / Skills: どのように考え、何ができるか
- Behavior / Actions: 何をするか
- State: 何を現在の状態として持つか
- Relations: 他のAgent / Systemとどう関係するか

内容は対象repoから観察できる範囲で記述し、存在しない能力や目的を創作しない。

## Principle

```
repo
  = entity + behavior + awareness
  = 実体 + 挙動 + 意識
```

これらは独立した部品ではなく相補的なAgentの側面である。

Skillはactionだけを意味しない。思考、観察、分類、仮説生成などもAgentのSkillになり得る。

## Scope

agentify自身の仕事は「repoを読んでagent.mdを作る」ことだけ。
