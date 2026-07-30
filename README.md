# LLM-Effort Study: Data and Analysis

This repository contains the dataset and analysis code for an empirical study on **human–LLM collaboration effort in software development tasks**.  
The study investigates how **traditional effort estimation metrics** compare with **Hybrid Intelligence Effort (HIE)** dimensions, capturing human oversight, iterative prompting behavior, and LLM reasoning complexity.


---

## Citation

If you use this dataset or code in your research, please cite the following paper:

```bibtex
@article{alaswad2026hybrid,
  title={Hybrid intelligence effort for software effort estimation in LLM assisted development},
  author={Alaswad, Feisal and Poovammal, E and Ramana, Kadiyala and Narayana, G Surya and Khan, Arfat Ahmad and Faheem, Muhammad},
  journal={Discover Computing},
  volume={29},
  number={1},
  pages={424},
  year={2026},
  publisher={Springer}
}
```

---


## Dataset Description

The dataset consists of two primary CSV files:

- **`Devs.csv`**  
  Anonymized developer metadata used for grouping and mixed-effects modeling.

- **`Task_execution_observations.csv`**  
  Task-level execution data, including:  
  - LLM model used  
  - Story Points and traditional effort indicators  
  - Interaction indicators (prompt iterations, corrective prompts, context augmentation)  
  - Human effort indicators (validation time, manual corrections, integration time)  
  - Code change indicators (modified files and modules)

---

## Analysis Code

The `code/` directory contains three Jupyter notebooks:

1. **`traditional_effort_analysis_llm_context.ipynb`**  
   Analysis of traditional effort estimation metrics in LLM-assisted development contexts.

2. **`hybrid_intelligence_vs_traditional_estimation_analysis.ipynb`**  
   Comparative analysis between traditional effort estimation and Hybrid Intelligence Effort (HIE) dimensions.

3. **`dominant_hybrid_intelligence_drivers_analysis.ipynb`**  
   Identification of dominant HIE drivers influencing overall development effort.

These notebooks include:
- Data cleaning and preprocessing  
- Computation of Hybrid Intelligence Effort indicators  
- Regression and linear mixed-effects modeling  
- Visualization of empirical results  







---

## Requirements

- Python 3.10+  
- pandas  
- numpy  
- statsmodels  
- matplotlib  
- seaborn  

---

## Usage

```bash
cd code/
jupyter notebook
```

Open the desired notebook and ensure the CSV files in the directory are correctly referenced.

---

## License

This project is licensed under the **MIT License**.  
See the `LICENSE` file for details.
