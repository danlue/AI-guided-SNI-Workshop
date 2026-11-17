# Data pack

The files are in the [Releases](https://github.com/YOUR-USERNAME/AI-guided-SNI-Workshop/releases), not in this repository. Download `SNI_workshop_pack.zip` and unzip it.

## Contents

| Folder | What it contains | Used in |
|---|---|---|
| `models/` | 10 AlphaFold 3 hexamer models (CIF, model 0 each) | guides 1, 2 and 3 |
| `confidences/` | Summary confidence files (JSON), with the ipTM | guides 2 and 3 |
| `pae/` | PAE of each model as a small protein-only array (`*_uint8x8.npz`), a preview picture, and the full PAE (`*_full_data_0_slim.json`) for NbNRC2a and NbNRC7a for ChimeraX | guides 2 and 3 |
| `reference/` | Cryo-EM structures of three known NRC resistosomes (9FP6, 9RI9, 9CC8) | background |
| `sequences/` | CC-NB-ARC sequences of the ten proteins (FASTA) | guide 1 |
| `job_requests/` | The 2024 AlphaFold Server job requests of the ten models | background |

The proteins are CaNRC8, CaNRC9, NbNRC2a, NbNRC3, NbNRC4c, NbNRC7a, SlNRC0, SlNRC1, SlNRC5 and SlNRC6.

## Source and changes

The models come from Zenodo [10.5281/zenodo.11546022](https://doi.org/10.5281/zenodo.11546022) (`NRCs.zip`, June 2024 AlphaFold 3 server jobs). To keep the pack small, only model 0 of each hexamer was kept, PAE was reduced to the protein part and stored as 8-bit values (PAE in angstrom times 8), and the full PAE file was kept only for the two proteins used in ChimeraX.

## Good to know

- These models were made with 50 oleic acid molecules. The live modelling in the guide uses 25, so the ipTM of a live job differs slightly from the value in the pack.
- AlphaFold Server outputs are for non-commercial use.

## Second download: Colab data

`SNI_workshop_colab_data.zip` (about 80 MB) holds only what the AI part needs: models, confidences and the PAE arrays. The Colab notebook downloads it automatically.
