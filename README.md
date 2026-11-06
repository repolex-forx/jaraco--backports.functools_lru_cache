# Repolex Knowledge Graph of jaraco/backports.functools_lru_cache

RDF knowledge graph data for [jaraco/backports.functools_lru_cache](https://github.com/jaraco/backports.functools_lru_cache), parsed by [repolex](https://repolex.ai).

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
rlex download jaraco/backports.functools_lru_cache
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 22ad4cd0ec15645ed75c1ee5e1d664a25b8e5795
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 22ad4cd0ec15645ed75c1ee5e1d664a25b8e5795
│           └── chunk-001.nq.gz
├── blob
│   ├── 06278c07530e5ab391b3bc453771c6882ffc1259.nq.gz
│   ├── 0c0937956fef01a6a1326f3b94da442c39b75964.nq.gz
│   ├── 1da7c192092793349b00dfdaba167fbb59a7a924.nq.gz
│   ├── 1f2aa7533b0423a8eb943f6f4ec02498e39581a0.nq.gz
│   ├── 2e3f4dd791a6372b427d618eb0baa8c4dc58e5f0.nq.gz
│   ├── 304196f81e11a168c9894f966e4a617ebf4ed53c.nq.gz
│   ├── 54c9000ec94341dd65c2053251b85b124017b9b5.nq.gz
│   ├── 54cc8303b22089e12053e552d4e6cb852a865b8a.nq.gz
│   ├── 577e87a793a20e413f7321f4f17ec1eba2ea1962.nq.gz
│   ├── 5bdc232005af9be104a00437ae9bc64417a4c1cc.nq.gz
│   ├── 5c05f9e27d57a4b7a3c3a9fdfecf8cddb8be499f.nq.gz
│   ├── 5eb3aa507b3f9b1641a0ca0b0d2d2ba067195f50.nq.gz
│   ├── 63a71a01800b6aa06dc93a05fd6c175f3daed662.nq.gz
│   ├── 69e3be50dac40cddced86e9df2f9c2df5a75f004.nq.gz
│   ├── 700235be57c1b2872455c0be5333f59cf568e252.nq.gz
│   ├── 724370638fc188317bbc7dc868f1a571995fd796.nq.gz
│   ├── 80b3e152d20c3a97cbdfbd2aedb7cd5edfb51a06.nq.gz
│   ├── 9a0f3bce1395ae3819030b822e5d9076c85068ea.nq.gz
│   ├── d226e149623898a43f35ab57295bb82004dc7d8d.nq.gz
│   ├── dc49a7455ee0c656f010b6a8935df3114d7f3982.nq.gz
│   ├── e05a3d4a2ab888e32952006d8cd380864368db5f.nq.gz
│   ├── e14c0f16a5f859ec7ece201d35bc34acfa42e5be.nq.gz
│   ├── e4391cf8a4301cbf5a00a64c1b4e687bfaf0562a.nq.gz
│   └── efcb8cbc2043faa7caf4f92fc7488bd6914c934c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 22ad4cd0ec15645ed75c1ee5e1d664a25b8e5795.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 32 files
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

[jaraco/backports.functools_lru_cache](https://github.com/jaraco/backports.functools_lru_cache)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
