# Repolex Knowledge Graph of astropy/quantity-2.0

RDF knowledge graph data for [astropy/quantity-2.0](https://github.com/astropy/quantity-2.0), parsed by [repolex](https://repolex.ai).

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
rlex download astropy/quantity-2.0
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c0d69c7c323d3b5ea69652d2fede4cda20ee0bca
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── c0d69c7c323d3b5ea69652d2fede4cda20ee0bca
│           └── chunk-001.nq.gz
├── blob
│   ├── 0ef4d412d1be7f57793445a3d1192b92e3d27a13.nq.gz
│   ├── 0f7aad4a66fba94e0a783259f17e6e462c5ddf87.nq.gz
│   ├── 109aaf9d6e086a3c6857e412cc3e9ad0d4b1d5a6.nq.gz
│   ├── 17c83dc040e2cfcdb6fa14174e948ea565410f5c.nq.gz
│   ├── 2119f51099bf37e4fdb6071dce9f451ea44c62dd.nq.gz
│   ├── 25033b7c19cbff0a12de5fa43906814b67e3d959.nq.gz
│   ├── 37054782ee950b26c44ff40523c09c187b55de00.nq.gz
│   ├── 43b61583f3d31122e8e110ad5facd726eb369cbf.nq.gz
│   ├── 4e26fabb806f4c0fd72ebf720cdfefdd36663d84.nq.gz
│   ├── 556ab7cc1e428766b4a83e09127016f42c2b2e8a.nq.gz
│   ├── 56e206bbdbd111e52227813add61647b95328d4a.nq.gz
│   ├── 67b82f693f53cef785f9750c2c65c0bc3c191c8b.nq.gz
│   ├── 92ea707303e3d1f4b6fc3bb3446d173c4f8d3c10.nq.gz
│   ├── 933d8ab2f7f025d4616c94132c2237dffd23daa8.nq.gz
│   ├── 94aff2f7882b7e8da4619c71adee7d9a4a0c719b.nq.gz
│   ├── a35b0d6d7fdb8c7cf65badf1045173378c999843.nq.gz
│   ├── ab4ac26973bee4da8898f856c38c36e6850f3149.nq.gz
│   ├── c091c36b09a9dcb786d358652afe73406f2ea28b.nq.gz
│   ├── d0d1cf181f4a4b6f10dffac57aa0df2ff703db88.nq.gz
│   ├── d16f7755789b6ba7e3adcbc81a2f3fe2d525d743.nq.gz
│   ├── d4bb2cbb9eddb1bb1b4f366623044af8e4830919.nq.gz
│   ├── e2a914daddd4182e25b642e429a9a776ce3a0ab4.nq.gz
│   ├── eefd848ed85f4689769d50a2b274e4e9144c9e5b.nq.gz
│   ├── f163052a576c644862d7937d4a645c3a94a56965.nq.gz
│   ├── f29177b0b7bcc2c96b3a54858969f0edbd5032fe.nq.gz
│   └── fec747601a3142b6563d3b88cd67bd11c6741ba4.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── c0d69c7c323d3b5ea69652d2fede4cda20ee0bca.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 34 files
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

[astropy/quantity-2.0](https://github.com/astropy/quantity-2.0)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
