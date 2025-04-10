# Dominance varies at different time scales: R code and simulated data for dominance network analysis

This repository contains R code for constructing and analyzing dominance networks using adjacency matrices and weight/abundance data. The original project is based on observational data of animal interactions and dominance behavior. To protect sensitive information, we provide simulated example datasets that match the structure of the real data.

## 📂 Repository Structure

```
DominanceNetworkAnalysis/
├── data/
│   ├── fake_adjacency_matrix.csv         # Simulated adjacency matrix
│   └── fake_weights_abundance.csv        # Simulated weight and abundance data
├── R/
│   └── dominance_network_analysis.R      # Main analysis script
├── README.md
└── LICENSE
```

## 🧪 What This Code Does

- Loads and processes directed, weighted adjacency matrices.
- Constructs and visualizes dominance networks using `igraph`.
- Annotates nodes with species' weight and abundance.
- Calculates hub and authority scores.
- Applies the `Perc` package for dominance ranking simulations.
- Computes network indices (e.g., density, reciprocity, centrality).

## 📊 Example Visualization

The network plots show individuals as nodes. Node size reflects species weight, and node color intensity indicates abundance. Edge width and color represent interaction weight.

## 🔧 Requirements

The following R packages are used:

- [`igraph`](https://igraph.org/r/) – for network creation and analysis
- [`Perc`](https://cran.r-project.org/web/packages/Perc/index.html) – for probabilistic dominance and ranking analysis
- [`ggplot2`](https://ggplot2.tidyverse.org/) (optional, for any visual extensions)

Install them via:

```r
install.packages("igraph")
install.packages("Perc")
```

## 🚀 How to Run

1. Clone or download this repository.
2. Open the script in `R/R/dominance_network_analysis.R`.
3. Make sure the working directory points to the root of the project.
4. Run the script. It will load the data in `/data/` and produce visualizations and outputs.

## 📁 Sample Data

We provide two example files in the `data/` folder:
- `fake_adjacency_matrix.csv`: A 10x10 matrix representing directed interactions between individuals.
- `fake_weights_abundance.csv`: Contains species `Weight` and `Abundance` for node attribute mapping.

These datasets are entirely artificial and provided solely for reproducibility of the script.

## 🧬 About the Project

This code was developed for a scientific study on dominance hierarchies and social structure in free-living hummingbirds. The real data consist of observed agonistic interactions coded into adjacency matrices across different days and months.

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## ✉️ Contact

Ana Melisa Fernandes  
fernandesanameli@gmail.com
