# Pile experimental processing packs

This public repository contains signed catalogs and licensed model/data artifacts only. Pile application source remains private. All packs are experimental; none is recommended.

Prepared families: multilingual MiniLM extraction; news-trained English T5-small generation; extraction with a small frozen-encoder classifier trained on agent-reviewed Wikipedia passages. The classifier study has only three classes and lacks publisher isolation. mT5 XL-Sum is unavailable because noncommercial distribution restrictions have not been cleared.

The catalog is verified using an Ed25519 public key pinned in the Pile application. Files have immutable versioned names, declared byte lengths and SHA-256 values. Model artifacts cannot supply executable code.

## Sources and licenses

- MiniLM: sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2, revision e8f8c211226b894fcb81acc59f3b34ba3efd5f42, Apache-2.0. Downloaded directly from frozen Hugging Face URLs.
- T5-small CNN/DailyMail: farleyknight/cnn_dailymail-summarization-t5-small-2022-09-05, revision 6b3c7e1e42534961e618814499becde97c674933, Apache-2.0. Tokenizer from google-t5/t5-small revision df1b051c49625cf57a3d0d8d3863ed4d13564fe4. Export/quantization provenance accompanies the release.
- Authored multilingual concept definitions: CC0-1.0.
- Experimental frozen-encoder classifier: CC-BY-SA-4.0, with source URLs/attributions/review scope embedded in the artifact. Training data are public Wikipedia passages; no user documents are included.

Limited T5 checks found omitted qualifications. Tokenizer and runtime equivalence are execution checks, not evidence of general summarization quality. Physical-phone budgets and broad held-out quality must be established separately.
