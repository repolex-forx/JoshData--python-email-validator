# Repolex Knowledge Graph of JoshData/python-email-validator

RDF knowledge graph data for [JoshData/python-email-validator](https://github.com/JoshData/python-email-validator), parsed by [repolex](https://repolex.ai).

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
rlex download JoshData/python-email-validator
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 4ac100ec9a45dbb8432bc9bf7c49e96591854846
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 4ac100ec9a45dbb8432bc9bf7c49e96591854846
│           └── chunk-001.nq.gz
├── blob
│   ├── 058ccfd8fbf7f7cb7ddbcc812695e8e6d44e26e9.nq.gz
│   ├── 07b398ab9567ca2570c95a993eb65a8efae19ed9.nq.gz
│   ├── 107b08bb39ba69c7de2e37afdc91d60593cb415b.nq.gz
│   ├── 122e7a71fcd85a909f2321cda3d4b8495b913c80.nq.gz
│   ├── 15c2f578c02bb0e6208a1476df41eb470e644bb7.nq.gz
│   ├── 38d0741489213c5ed5de042f6efb81cbb08fc8a8.nq.gz
│   ├── 3cddc77cad7034564946768dc97778a0ec637f16.nq.gz
│   ├── 43508a3c0e4978a57055a41252328f0fb2e92215.nq.gz
│   ├── 44ccb2f943a1283f06e53a654964b2c2b83d6b6c.nq.gz
│   ├── 55e47090701a5a75058e8f54194356146af38fc4.nq.gz
│   ├── 57393374674cdd82b3d114253a5032a4e95c3aa9.nq.gz
│   ├── 57df9da493e2af3d5fbfa5d6994c0beec8ef934d.nq.gz
│   ├── 76e88b9ffc4c5b1b2464b77ce35b7623540d59de.nq.gz
│   ├── 87db51a1f79a8f4043dc7f2b1b73606e97e0e4fb.nq.gz
│   ├── 87ef13c5a1f50b51f5605164fe960d7cefc9da28.nq.gz
│   ├── 8bf1ba938af9b4993f625db4fc6e708be9f3f3b7.nq.gz
│   ├── 927591c9a357d5a3ad9015cf6a5c7788dded0b91.nq.gz
│   ├── a92c08eb270631aab0804181644e36bc02b381b2.nq.gz
│   ├── ad970d4b0430a738ce8dfcd40b52df5574e2f498.nq.gz
│   ├── b22c457cd9cb2d5faba2c3a11fa4137163b9f5f8.nq.gz
│   ├── b8c6583f593eece2b564b65a5fd4a7b71b0c3943.nq.gz
│   ├── c285d609df5ded20ce4410b0178dc2a3c0a72e88.nq.gz
│   ├── e1307c2b6827b8613284aa7233f4124410d762e1.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e88a3a4d4708ec8d8728111b2b7b35add02293a4.nq.gz
│   ├── e93441b2936714314da5e7bed23d113b1177f562.nq.gz
│   └── f7cb70d550bd5888501a78a4f3404a3cd7748b93.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 4ac100ec9a45dbb8432bc9bf7c49e96591854846.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 35 files
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

[JoshData/python-email-validator](https://github.com/JoshData/python-email-validator)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
