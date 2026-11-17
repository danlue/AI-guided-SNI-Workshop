# AI-guided Structural Novelty Index (SNI)

2026 Iwate NLR Biology Workshop and Mini-Symposium, Iwate Biotechnology Research Center, Iwate, Japan, 17–21 November 2026. A 50-minute hands-on session on building and using a structural novelty index, with optional hands-on work for participants.

| Part | Minutes | What we do | Guide page |
|---|---|---|---|
| Set-up (optional, before) | beforehand | Accounts, ChimeraX, data pack, Colab | 0 |
| **Live modelling** | 0–8 | Model an NRC hexamer in AlphaFold Server, look at it in ChimeraX | 1 |
| **ChimeraX by hand** | 8–25 | From a picture to numbers: confidence, contacts, buried area, geometry | 2 |
| **Build the pipeline with AI** | 25–42 | Turn metric definitions into a script with a free AI assistant in Colab | 3 |
| **Validate and discuss** | 42–50 | Heatmap, clustering, discussion | 4 |

Delivered by the Kamoun Lab, [The Sainsbury Laboratory](https://www.tsl.ac.uk/).

### Website: **https://danlue.github.io/AI-guided-SNI-Workshop/**

The step-by-step guide for participants (English and Japanese) is on the site: set-up, every command with a copy button and an explanation, the AI prompts, a glossary and the references. Taking part on your own laptop is optional; the instructor goes through every step on the screen.

---

## Downloads

- **Data pack:** [SNI_workshop_pack.zip](https://github.com/danlue/AI-guided-SNI-Workshop/releases/download/v0.1/SNI_workshop_pack.zip) (about 119 MB zipped). Ten pre-computed NRC hexamer models, their confidence files, and reference structures. See [data/README.md](data/README.md).
- **Colab notebook:** [colab/SNI_workshop_colab_setup.ipynb](colab/SNI_workshop_colab_setup.ipynb). It downloads a small data set (about 80 MB) for the AI part. A ready-to-open link is on the website.

## What is in this repository

```
index.html     the step-by-step guide (the website, served by GitHub Pages)
colab/         the Colab notebook (data set-up for the AI part)
data/          a description of the data pack; the files themselves are in the Releases
```

The data files are large, so they are attached to the [Releases](https://github.com/danlue/AI-guided-SNI-Workshop/releases) and are not stored in the repository itself.

## The data

The ten models are AlphaFold 3 predictions of the CC-NB-ARC region of NRC helper NLRs as hexamers, with oleic acid as a stand-in for the membrane. They come from the original Zenodo record, [10.5281/zenodo.11546022](https://doi.org/10.5281/zenodo.11546022) (`NRCs.zip`, June 2024 AlphaFold 3 server jobs, model 0 only). The pack is a slim version of that record. The parameter definitions are from the preprint. AlphaFold Server outputs are for non-commercial use; see the [terms](https://alphafoldserver.com/terms).

## Citation and sources

The workshop is based on the preprint: Toghani A, Seager B, et al. (2026), bioRxiv, [doi:10.64898/2026.05.03.722499](https://www.biorxiv.org/content/10.64898/2026.05.03.722499v1). The full list of references used in the guide is on the last page of the website.

## Questions

For anything about this workshop: daniel.luedke@tsl.ac.uk.

## Reuse

The teaching materials (guide, text, slides) are licensed under [CC BY 4.0](LICENSE). The code (notebook and scripts) is licensed under the [MIT licence](LICENSE-CODE). The AlphaFold models keep the AlphaFold Server terms (non-commercial use).

---

## 日本語の概要

「AI を活用した構造新規性指数（SNI）」の1時間のハンズオンです。AlphaFold Server でのモデリング、ChimeraX での解析、AI アシスタントを使ったパイプラインの構築、結果の検証を行います。ご自身のノートパソコンで操作するかどうかは任意で、講師がすべてのステップを画面上で説明します。英語・日本語のステップバイステップのガイドは、上のウェブサイトにあります（右上の **EN / 日本語** ボタンで切り替えられます）。コマンド、ファイル名、AI へのプロンプトは英語のままです。
