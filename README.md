# Heredity AI

This project calculates the probability that individuals in a family tree carry a gene and exhibit a trait, based on genetic inheritance and mutation. It uses **Bayesian networks** to perform probabilistic inference on real-world genetic relationships.


---

## Project Overview

Given a CSV file with family information (names, parents, and traits), the program:

- Computes the probability each person has **0, 1, or 2 copies** of a gene.
- Calculates the probability they **do or do not exhibit** a given trait.
- Considers **mutation** and **inheritance** probabilities.
- Outputs **normalized joint probabilities** for each person.

---

## Concepts Used

- Bayesian Inference
- Joint Probability Distribution
- Conditional Probability
- Genetic Inheritance & Mutation
- Normalization of Probabilities

---


---

## ▶️ How to Run

With python3 installed run the code bellow:

```bash
python3 heredity.py data/family0.csv
```

With older python version installed run the code bellow:

```bash
python heredity.py data/family0.csv
```

Example of input data

name,mother,father,trait
Harry,Lily,James,
James,,,TRUE
Lily,,,FALSE

Output

Harry:
  Gene:
    2 copies: 0.002
    1 copy:   0.409
    0 copies: 0.589
  Trait:
    Has trait:     0.033
    Doesn't have:  0.967


