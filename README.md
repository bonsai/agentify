# agentify

**Repository → Agent**

すべてのrepoをAgentとして扱うための最小Skill。

agentifyは対象repoを読み、そのrepoの**実体・挙動・意識**を相補的に捉えて、直下に `agent.md` を作る。

## Rule

`repoを読む → agent.mdを作る`

それ以外の成果物は作らない。

## Agent

- **実体** — repo、code、data、assets
- **挙動** — actions、workflows、skills
- **意識** — awareness、concern、purpose、attention

思考系の能力もSkillとして記述する。

## Output

```
target-repo/
└── agent.md
```

対象repoに既存の `agent.md` があれば、観察結果に基づいて更新する。

## Principle

> repo is an Agent.

> Agentの実体・挙動・意識は相補的である。
