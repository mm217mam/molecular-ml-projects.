# molecular-ml-projects.
Machine learning projects for molecular and materials science (RDKit, cheminformatics, and property prediction).

# Molecular ML Projects

Machine learning projects focused on molecules and materials, with an emphasis on cheminformatics, RDKit feature engineering, and property prediction models.

## Project 1 – AqSolDB Aqueous Solubility

**Goal.** Predict aqueous solubility (logS) in water for ~10k organic and inorganic compounds from the AqSolDB dataset using classical ML models on RDKit descriptors.

**Methods.**
- Curated AqSolDB and generated ~200 RDKit 2D descriptors per molecule.
- Trained several regressors (Random Forest, Gradient Boosting, MLP) and Morgan‑fingerprint baselines.
- Performed scientific error analysis vs. key descriptors (MolLogP, TPSA, MolWt) and inspected worst‑predicted molecules (metal salts, highly substituted chains, extreme chemotypes).

**Key results.**
- Best model: RDKit descriptors + Random Forest.
- Achieved ≈0.65 MAE and ≈0.96 RMSE on logS with strong R² on a 20% validation split.
- Largest errors occur for very low‑solubility compounds and complex metal salts where 2D descriptors underrepresent speciation.

**Resources.**
- Kaggle notebook: \<[a](https://www.kaggle.com/code/montesmiguel/project1-aqsoldb-solubility)>
- Dataset: AqSolDB – A curated reference set of aqueous solubility data.

---

More molecular ML projects (e.g., GNNs for molecular property prediction, protein–ligand modeling) will be added to this repository over time.
