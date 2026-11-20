# DCC Pro-Seminar course files

Data and code for the guide [Getting Started with the Duke Compute Cluster](https://wenhaojiangsoc.github.io/blog/2026/duke-compute-cluster/), Duke Sociology Pro-Seminar, November 20, 2026.

| File | What it does |
| :-- | :-- |
| `demo.R`, `demo.sh` | College wage premium regression, run as one job |
| `boot.R`, `boot.sh` | 100 bootstrap draws as a job array |
| `combine.R`, `combine.sh` | Bootstrap standard errors from the array's results |
| `mnist.py`, `mnist.sh` | Small neural network on MNIST, on a GPU |
| `logs/`, `results/` | Where jobs write their output |

## Data

- `data/acs_nc_2024.csv`: U.S. Census Bureau, [American Community Survey](https://www.census.gov/programs-surveys/acs/microdata.html) 2024 1-year Public Use Microdata Sample, North Carolina person file, all 114,270 records, 17 variables. Public domain.
- `data/MNIST/raw/`: the [MNIST](https://en.wikipedia.org/wiki/MNIST_database) handwritten digits (LeCun, Cortes, and Burges), 60,000 training and 10,000 test images, in the layout PyTorch's `torchvision.datasets.MNIST` expects. Licensed CC BY-SA 3.0.
