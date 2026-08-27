# ECE 2112: Experiment 2 - Numerical Python (NumPy)

This repository contains the solution notebook and generated binary output files for Experiment 2 of ECE 2112 (Advanced Computer Programming and Algorithms) at the University of Santo Tomas.

## Author Details
* **Name:** Adrian Joseph R. Herrera
* **Section:** 2ECE-D
* **Student ID:** 2025000458

## Intended Learning Outcomes
* Apply vectorized array operations and matrix transformations using NumPy.
* Perform statistical operations (mean, standard deviation) across multi-dimensional arrays.
* Implement relational logic and Boolean masking to filter array elements without explicit loops.
* Utilize binary file I/O (`.npy`) for persistent array storage and data retrieval.

## Programming Problems Covered
* **Problem A: Reproducible Matrix Normalization (`X_normalized.npy`):** Constructs a $5 \times 5$ uniform random matrix using a fixed random seed (`np.random.seed(2112)`). Standardizes the matrix into $Z$-scores using standard score transformation:
  
  $$Z = \frac{X - \mu}{\sigma}$$
  
  The resulting standardized array is saved as a binary file.

* **Problem B: Cubes Divisible by 4 (`div_by_4.npy`):** Generates a $10 \times 10$ array containing consecutive integers from $1$ to $100$, applies element-wise cubing ($x^3$), and uses modulo Boolean masking (`% 4 == 0`) to extract elements divisible by 4 into a 1D array.

* **Problem C: Above-Mean Squares (`above_mean.npy`):** Formulates a $6 \times 6$ matrix of squared consecutive integers ($1^2$ to $36^2$), calculates the global matrix mean, and utilizes relational slicing (`> mean`) to isolate elements strictly greater than the overall average.

## Repository Contents
```text
.
├── ECE2112_Exp2_Herrera.ipynb    # Primary Jupyter Notebook solution
├── X_normalized.npy              # Binary output for Problem A
├── div_by_4.npy                  # Binary output for Problem B
├── above_mean.npy                # Binary output for Problem C
└── README.md                     # Repository documentation
