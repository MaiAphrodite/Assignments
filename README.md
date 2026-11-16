# Assignments

> Course assignment storage, currently one Big Data practicum set in Jupyter

[![License](https://img.shields.io/badge/license-MIT-2ea44f?style=flat-square)](LICENSE)
[![Stack](https://img.shields.io/badge/stack-Jupyter%20%2B%20PySpark-F37626?style=flat-square)](#notebooks)

This repository is where course assignments live. Right now it holds the first Big Data practicum: three notebooks that walk through Big Data basics, Spark DataFrames, and Pandas, plus the screenshots the practicum embeds. Nothing here is a product, the notebooks are coursework, and some cells are still exercise prompts with the answer left as a task.

Open them with `jupyter lab` from inside `BigData/`. The package list and caveats are further down.

## Notebooks

| File | Topic |
|------|-------|
| `BigData/Praktikum 1 Big Data.ipynb` | The finished practicum write-up: Big Data concepts, Anaconda and environment setup with screenshots, Spark DataFrame creation, filter and average and sort, Pandas merge, and a Matplotlib chart themed with catppuccin |
| `BigData/Hands_On_Pertemuan_1.ipynb` | The hands-on companion sheet: same flow with fewer illustrations, mostly step-by-step instructions plus a few starter code cells (Spark DataFrame, Pandas DataFrame, conversions) |
| `BigData/MEong220` | A Google Colab export doing a PySpark sales analysis: a revenue column from quantity times price, revenue grouped by year and month and category, cheapest product per category, monthly quantity trend, and a revenue-per-category bar chart |

`BigData/images/` holds eleven screenshots, ten of which `Praktikum 1 Big Data.ipynb` embeds, so open the notebook from inside `BigData/` or the image links break. `MEong220` has no `.ipynb` extension: copy it to `MEong220.ipynb` if you want Jupyter to open it by double click.

## How to open

Any Jupyter environment works. From the `BigData` directory:

```bash
jupyter lab
```

The notebooks import `pyspark`, `findspark`, `pandas`, `matplotlib`, and `catppuccin`, and Spark needs a Java runtime. There is no requirements file in the repository, so install those yourself or run the notebooks in Colab, which is how `MEong220` was produced.

The Markdown is in Indonesian, matching the course language, and `Praktikum 1 Big Data.ipynb` explains each code block line by line.

## Notes and limitations

- Coursework scope: several cells are tasks ("Tugas 1", "Tugas 2", and so on) rather than finished answers, and `Hands_On_Pertemuan_1.ipynb` has empty code cells.
- No locked environment, no `requirements.txt`, and no test harness. Outputs may not match a fresh install, especially Spark version differences.
- `MEong220` was exported without the `.ipynb` extension and starts with `!pip install pyspark pandas`, which only makes sense in a Colab or notebook shell.

## License

MIT, see [LICENSE](LICENSE).
