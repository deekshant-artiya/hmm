# Hidden Markov Model (HMM) & Viterbi Decoding

This project implements a **Hidden Markov Model (HMM)** from scratch to solve the "decoding problem" using the **Viterbi Algorithm**. It demonstrates how to predict a sequence of hidden (unobserved) states based on a series of observed events.

## Project Overview

An HMM is a statistical model used to describe the evolution of observable events that are influenced by internal, "hidden" factors. The Viterbi algorithm is the standard dynamic programming approach used to find the "Viterbi path" the most likely sequence of hidden states given the observed data.

### Core Concepts:
* **Hidden States:** The actual process we want to discover (e.g., Weather: Sunny/Rainy).
* **Observations:** The data we can actually see (e.g., Activity: Walking/Cleaning).
* **Transition Probabilities:** The likelihood of moving from one hidden state to another.
* **Emission Probabilities:** The likelihood of a specific observation occurring given a hidden state.

## Files Included

* `viterbi_analysis.py`: A clean, object-oriented Python implementation using NumPy for matrix operations.
* `Assignment_HMM_and_Viterbi.ipynb`: Documentation and experimental results.
* `README.md`: Project description and setup instructions.

## How It Works

The implementation follows a professional **Object-Oriented Programming (OOP)** structure. The `HMMViterbi` class handles the model parameters and executes the algorithm in three phases:

1.  **Initialization**: Calculates the starting probabilities for the first observation.
2.  **The Forward Pass (Trellis)**: Fills a probability matrix (trellis) using the Markov property—where the current state depends only on the previous state.
3.  **Backtracking**: Once the full sequence is processed, the algorithm "walks backward" through the most likely path to determine the hidden state sequence.

## Tools & Libraries

* **Python 3.x**
* **NumPy**: Used for efficient matrix storage and `argmax` operations.

## Running the Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/deekshant-artiya/hmm
   cd hmm
