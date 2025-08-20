# SecuritySyntheticImages

**Synthetic radiograph generation, reader study, and detection tooling**

This repository hosts code and notebooks for our study on (1) generating synthetic radiographs, (2) reader performance vs. timing, and (3) basic safeguards (cryptographic signatures, provenance checks) to mitigate misuse. We provide reproducible analyses for two balanced datasets: **154 images** (77 GPT‑generated, 77 real) and **110 images** (55 RoentGen synthetic, 55 real).

---

## Contents

* `Cryptography/crypto.ipynb` — Examples of provenance tooling (hashing, signing, simple watermark checks) for synthetic radiographs.

> **Note**: The repository currently includes the cryptography notebook. 

---

## Quick start

### 1) Environment

```bash
# Python 3.10+
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

Minimal requirements (if you are running notebooks only):

```
pandas
numpy
statsmodels
scipy
scikit-learn
matplotlib
jupyter
```

### 2) Open notebooks

* GitHub renders notebooks in‑browser. To run interactively:

  * **Colab**: open the notebook link and replace the URL prefix with `https://colab.research.google.com/github/...`
  * **Jupyter**: `jupyter lab` or `jupyter notebook` from the repo root.

---

## Data

At present, no image data or metadata tables are shipped in the repository. The cryptography notebook operates on example payloads generated within the notebook. 

---

## Analyses (planned)

The repository contains `Cryptography/crypto.ipynb`.


---

## Security & provenance

See **`crypto.ipynb`** for examples on hashing, signing, and basic watermark/provenance checks intended to reduce the risk of synthetic images being misused or inserted into clinical systems.

---

## Regulatory considerations (brief)

Synthetic medical imaging intersects with **SaMD** pathways (e.g., FDA 510(k)/De Novo; EU MDR). Key issues: **validation**, **labeling/disclosure**, **privacy**, **misuse prevention**, and **post‑market surveillance**. We discuss these in the manuscript’s Discussion.

---

## Citation

If you use this repository, please cite:

```
Tordjman M, Ozkaya E, Yuce M et al. SecuritySyntheticImages: Synthetic radiographs, reader study, and safeguards. 2025. GitHub repository.
```

---

## Contributing

Issues and pull requests are welcome. Please avoid uploading any identifiable patient data.

---

## License

Apache 2.0

---

## Contact

Open an issue on GitHub or reach out via the repository contact listed in the profile.
