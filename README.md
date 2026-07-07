# Randomness Analysis

This project compares different ways of generating random bits using Python.

The project looks at three random bit sources:

1. Algorithmic random bits
2. Atmospheric random bits
3. Quantum random bits

The goal is to collect random bit samples, run statistical tests on them, and compare the results using graphs.

## What This Project Does

This project:

1. Generates or collects random bits
2. Cleans the data into CSV files
3. Runs statistical tests on the bit sequences
4. Compares the results across different random number sources
5. Creates graphs to visualize the results

## Random Bit Sources

### Algorithmic Random Bits

These bits are generated using Python's built in random number tools.

### Atmospheric Random Bits

These bits come from atmospheric noise data from Random.org.

### Quantum Random Bits

These bits come from quantum random number data from the ANU Quantum Random Numbers API.

## Statistical Tests Used

This project uses three main tests.

### Frequency Test

This test checks whether the number of 0s and 1s are close to equal.

A balanced 10,000 bit sample should have about 5,000 zeros and 5,000 ones.

### Runs Test

This test checks whether the sequence switches between 0s and 1s in a way that looks random.

A sequence with too many repeated values or too many changes may be less random.

### Serial Correlation

This checks whether each bit is related to the bit that comes after it.

A random sequence should have very little correlation between neighboring bits.

## Project Structure

```text
randomness-analysis/
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
├── code/
│   ├── single_trial/
│   └── multi_trials/
├── data/
│   └── single_trial/
├── results/
│   └── multi_trials/
├── graphs/
│   ├── single_trial/
│   └── multi_trials/
└── notes/
