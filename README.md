# Repolex Knowledge Graph of plotly/dash-player

RDF knowledge graph data for [plotly/dash-player](https://github.com/plotly/dash-player), parsed by [repolex](https://repolex.ai).

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
rlex download plotly/dash-player
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d663df9ccbb5c5c009ce77d1f01542d92a133ad5
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── d663df9ccbb5c5c009ce77d1f01542d92a133ad5
│           └── chunk-001.nq.gz
├── blob
│   ├── 0471d7b14c897130a4637bd4f8511a751465408a.nq.gz
│   ├── 0bb1753afa634b98fe05d36c31fdc3425a5e3ff5.nq.gz
│   ├── 0ff865a571c506d2333e7f166acdbf5fa5df5ad6.nq.gz
│   ├── 14597d808b916a54088c8a3a8eae0e4cdb142d3e.nq.gz
│   ├── 197d4dbd0c8ec7a382eacc46bfd7749771e8d334.nq.gz
│   ├── 208c8d7151ddf6e6f43493498c7d9e4caa64d671.nq.gz
│   ├── 2be747dfd2c86255938ebb332ba41460eceadda4.nq.gz
│   ├── 2ff2c3db521ddc6b370ab0282ff3ae34fce12e49.nq.gz
│   ├── 41e5c017218cc543d444a308a7c503c64f58fcdc.nq.gz
│   ├── 56935b247a5295fcce9f94e9b8367985d905e877.nq.gz
│   ├── 57970d14a9881d8df9e35b23e8f4ef7e9f1e9a34.nq.gz
│   ├── 5832d48a77b062fc2a6bb93fc6ef213aa48487d8.nq.gz
│   ├── 595be2c724e0c285fe4b7713b4463628ab17a2f5.nq.gz
│   ├── 5b547f38355bef0555bf4e9b860d020f7d71e798.nq.gz
│   ├── 61e63400fbca91668fa11457bb155ddb315cd9f8.nq.gz
│   ├── 61ff53684313c399a00f12b6f22d2477b56d4ccc.nq.gz
│   ├── 6ddf014ba956cb6ec41bde98f7bfed7599150bad.nq.gz
│   ├── 6f1019e2e290f289e8fc4228a22b068abc498aa8.nq.gz
│   ├── 707df5b0933f967a3abb61c34e6fd71ec290f8e8.nq.gz
│   ├── 7420bf10f13823969041a2977a02e1c3297e5728.nq.gz
│   ├── 74234c03285f5e3ef3dd676ca24267736865e920.nq.gz
│   ├── 75e9b317940d32eee3e52437e62118946a6fede0.nq.gz
│   ├── 802ea345fd3896fd95d92a7a1df6fc8d7c6a49e8.nq.gz
│   ├── 8cf7af30d0a91e6de7916174ff91ac8d28d5f2a5.nq.gz
│   ├── 9819a45d04d38b2dba1e0207eba03fc2863f1eaf.nq.gz
│   ├── 9c381ced5e8c12d0b117417359aca741d96d143c.nq.gz
│   ├── 9c5cf0b2056ecb521b8e363b7b03202bf0d40a5c.nq.gz
│   ├── 9fb695f0d7ad20a8fcb70d52180e86fd92f71bfc.nq.gz
│   ├── aeeee4ea9a5b5f7a2cbd3f62b34ce22702618124.nq.gz
│   ├── b1bb721755756cd3e43a02d86f513f189ce2e3c6.nq.gz
│   ├── b597a44232c2a3b77943c95857fa5c6075cf69d8.nq.gz
│   ├── bc8371522911dae5c57fa15028a9c84eeb316709.nq.gz
│   ├── c0beaf81d55c05f8b9c50e4f66eba9c4b3bd1745.nq.gz
│   ├── c98659ae7916568a2839104263067dd19cbcd845.nq.gz
│   ├── ca38e4f8035163a706ed073a33d55b0cf4bbf9a8.nq.gz
│   ├── d056d8dbfd56a3382585b390dc7da7fc33659683.nq.gz
│   ├── d80f52b789ce181b0cb1c2b89f656e54fca2d6c0.nq.gz
│   ├── dbd8407b1d2e6d9b101b58913a0e8fb8b44a674f.nq.gz
│   ├── e01c5b9573f792580cb3733cfbe8cc94bb3c7cfd.nq.gz
│   ├── e4ad325dfc318ba075a1e04a440fe37096f54eeb.nq.gz
│   └── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── d663df9ccbb5c5c009ce77d1f01542d92a133ad5.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[plotly/dash-player](https://github.com/plotly/dash-player)

---
*Parsed on 2026-11-07 by [repolex](https://repolex.ai)*
