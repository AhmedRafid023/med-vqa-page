# BanglaMedVQA — Project Page

Official project page for the ACL 2026 paper:

> **Evaluating Large Vision Language Models on Bangla Medical Visual Question Answering**  
> Rafid Ahmed, Intesar Tahmid, Mir Sazzat Hossain, Tasnimul Hossain Tomal, Md Mahir Jawad, Anam Borhan Uddin, Md Fahim, Md Farhad Alam Bhuiyan  
> *Association for Computational Linguistics (ACL 2026)*

🔗 **Live Site**: [AhmedRafid023.github.io/med-vqa-project-page](https://AhmedRafid023.github.io/med-vqa-project-page)  
📄 **Paper**: [Google Drive](https://drive.google.com/file/d/1SUm9jwgp2cxegX2v9om03jqw3jm1dy3i/view?usp=drive_link)  
💻 **Code**: [med-vqa-LoRA](https://github.com/AhmedRafid023/med-vqa-LoRA)  
🗄️ **Dataset**: [BanglaMedVQA on HuggingFace](https://huggingface.co/datasets/iiCEMAN/BanglaMedVQA)

---

## About

We introduce **BanglaMedVQA**, a multilingual Medical Visual Question Answering (VQA) benchmark comprising clinically validated image–question–answer pairs for the Bangla language. We rigorously evaluate nine state-of-the-art Large Vision Language Models (LVLMs) using zero-shot, Chain-of-Thought (CoT), and LoRA fine-tuning strategies.

---

## Features of This Project Page

- 📊 **Interactive LAVE Score Comparison** — bar chart comparing all 9 models across Bangla & English QA pairs
- 🕸️ **Interactive Radar Charts** — category-level performance breakdown (Modality, Organ, Abnormality, Condition, Position) for Zero-Shot, CoT, and LoRA
- 🌙 **Dark / Light Mode Toggle** — fixed button in the top-right corner
- 📋 **Full Benchmark Tables** — color-highlighted HTML tables for Bangla and English results
- 📁 **Dataset Distribution** — interactive organ-wise sunburst and keyword frequency charts

---

## Local Development

**Requirements**: Node.js ≥ 18.20.8

```bash
# Install dependencies
npm install

# Start dev server
npm run dev
```

The site will be available at `http://localhost:4321`.

---

## Deployment

This site is automatically deployed to **GitHub Pages** via the included GitHub Actions workflow whenever changes are pushed to the `main` branch.

To deploy manually:

```bash
git add .
git commit -m "update"
git push origin main
```

---

## Project Structure

```
src/
├── paper.mdx                    # Main content file
├── pages/index.astro            # Page shell (header, footer, theme toggle)
└── components/
    ├── InteractiveChart.astro   # Bar chart: overall LAVE comparison
    ├── InteractiveRadarCharts.astro  # Radar charts: category performance
    ├── TableBangla.astro        # Benchmark table for Bangla results
    └── TableEnglish.astro       # Benchmark table for English results
public/
└── images/                      # PDF figures and radar charts
```

---

## Citation

```bibtex
@inproceedings{ahmed-etal-2026-banglamedvqa,
  title     = {Evaluating Large Vision Language Models on Bangla Medical Visual Question Answering},
  author    = {Ahmed, Rafid and Tahmid, Intesar and Hossain, Mir Sazzat and Tomal, Tasnimul Hossain and Jawad, Md Mahir and Uddin, Anam Borhan and Fahim, Md and Bhuiyan, Md Farhad Alam},
  booktitle = {Proceedings of the 64th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)},
  month     = aug,
  year      = {2026},
  address   = {San Diego, California, USA},
  publisher = {Association for Computational Linguistics}
}
```

---

© Copyright 2026 Rafid Ahmed.
