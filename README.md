# Repolex Knowledge Graph of tiangolo/poetry-version-plugin

RDF knowledge graph data for [tiangolo/poetry-version-plugin](https://github.com/tiangolo/poetry-version-plugin), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download tiangolo/poetry-version-plugin
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 96835bf262405f332cc8f020db86a5ce5992091b
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 96835bf262405f332cc8f020db86a5ce5992091b
│           └── chunk-001.nq.gz
├── blob
│   ├── 0045fb8182cf94a55db192aa3bc8c4c7e033da47.nq.gz
│   ├── 034f46c34d93f457811adaa9a1e08de3ed4be752.nq.gz
│   ├── 0500a1a08f7c9cd20118480f89c1594eb9956f73.nq.gz
│   ├── 0ffc101a3f23548392499fe5104f3f8cf4d4e91b.nq.gz
│   ├── 108745ca4583f9d9fee42a4b00960a79933422da.nq.gz
│   ├── 10cc8c03f306edd186ed576504d44dd31b5b950c.nq.gz
│   ├── 128d8d60469e31fbf136e6b3455c3fa153b83878.nq.gz
│   ├── 1308fa8a619b2fc58e6c1bd4ae9fa61da5fb0925.nq.gz
│   ├── 162c2dc21b3d42962089a6ca0b0f20a1bdb988f3.nq.gz
│   ├── 1bc08279d8c1af7841bedecb4d8e6721fb1a6667.nq.gz
│   ├── 223d307a7c4ee9d2cbabad76c04a404162c4b3a4.nq.gz
│   ├── 2b272d5117adb170bf6ca41b062bf9ffe709f39e.nq.gz
│   ├── 3b93d0be0c9ec9943a1076a0152b8c244261a3a1.nq.gz
│   ├── 4f0044509a75af1fad470b3fdd0d1677d75b33f7.nq.gz
│   ├── 6467009a10093a787164548680e65849c8459799.nq.gz
│   ├── 6526deb4287620e5f1c9db3644c0e32520cd2983.nq.gz
│   ├── 7172e25d44860c34c5430adff5667b8e208df25c.nq.gz
│   ├── 72d5fe9b142692717fec2ebf0fa28eacb09ce2a6.nq.gz
│   ├── 7c41bf8e865d11775a2bbf9c5ed8efdf7605ea5a.nq.gz
│   ├── 81f0fdeccf66f1b74184b96bd53b64be1b903aae.nq.gz
│   ├── 905a3df851f1b944e6e6fe3d74d386bbccb8e779.nq.gz
│   ├── 91dba3a23c5b183103cd9db38ae3d4615e00c0d3.nq.gz
│   ├── 9903b2a9256bc1b592bb0b325f7771d592c13dbc.nq.gz
│   ├── a2ad41615e0079a6a61df26db4b81107d29636da.nq.gz
│   ├── a73339bf81370efc24e667e80c0cd6d8b8b80687.nq.gz
│   ├── a863dc70344be5b1fc157d03271698a50746aa6c.nq.gz
│   ├── acc716ded6ab9c194099c324fad09325de9ae9ac.nq.gz
│   ├── b18da3b241e37e94c6d706328d36b2ab6cbe446a.nq.gz
│   ├── b1a19e3237d1144638816320f076a5752ef36ef5.nq.gz
│   ├── b3c5111e6500ebb81d1672fe6f8a5e1d63831b60.nq.gz
│   ├── b52d88ed6ca72705d858a2813cf4f668bf416c44.nq.gz
│   ├── bdc67d7515dd9a72f81890ac57eaa075be7dc765.nq.gz
│   ├── c11870fac8e15a48256cd22373b015ee3a7d1a8f.nq.gz
│   ├── cd972a0ba47221bf96acedfaed8f3b5cba819849.nq.gz
│   ├── ce0dfd0a20f141675db00cfecbfe53e7d0ecd08a.nq.gz
│   ├── dba7b7a88940c992b6e170828611d27b01206a5a.nq.gz
│   ├── e25ad81f55f3c79fc28010288bce7449339481eb.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f102a9cadfa89ce554b3b26d2b90bfba2e05273c.nq.gz
│   └── fdcb5707dfe2662a007c81ab2fa00827cdebccbc.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 96835bf262405f332cc8f020db86a5ce5992091b.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[tiangolo/poetry-version-plugin](https://github.com/tiangolo/poetry-version-plugin)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
