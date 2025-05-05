# Optimization Approaches for Multi-Product Batch Purchases in Different E-Commerce Platforms

This repository contains the resources related to the master's degree research entitled **"Optimization Approaches for Multi-Product Batch Purchases in Different E-Commerce Platforms"**.

## Description

The research investigates and compares different optimization strategies for purchasing multiple products in batches across various e-commerce platforms. The goal is to minimize overall cost and/or maximize efficiency by considering platform-specific constraints and pricing schemes.

## Abstract
The problem of purchasing multiple items from various suppliers involves minimizing the total acquisition cost of a set of products available across different vendors. Key factors such as shipping costs, item availability, unit price, and quantity offered by each supplier are taken into account. This is a combinatorial optimization problem with exponential computational complexity. In this research, suppliers are represented by online retailers, and the problem is considered to be solved on a web server. The objective was to identify mechanisms capable of solving the problem while reducing computational costs compared to deterministic methods, with an emphasis on applicability in web-based environments.

To address this challenge, four heuristic optimization approaches were proposed, implemented, and evaluated for their ability to approximate the minimum total cost. These approaches were benchmarked against the exact solution derived using Integer Linear Programming (ILP), which becomes computationally infeasible as the search space grows. The heuristics investigated include: the Greedy approach, Greedy Reduction, Divide and Conquer, and a Genetic Algorithm.

Experiments were conducted using purchase orders containing varying numbers of products. Two datasets were employed: a real dataset reflecting the inventory conditions of 177 e-commerce stores, and a synthetic dataset that extends the real one by assuming full stock availability from all suppliers. Results—including convergence times and solution quality—were analyzed to compare the proposed approaches. All heuristics reached solutions significantly faster than the exact method. The Greedy approach had the fastest convergence but produced higher-cost solutions. Greedy Reduction generally achieved the lowest costs but required longer runtimes. Divide and Conquer yielded intermediate performance in both solution quality and execution time. The Genetic Algorithm, however, was unable to consistently converge to optimal or near-optimal results within the given time limits, indicating its unsuitability for this specific problem.

## Contents

- 📂 **datasets**: Contains the real and synthetic datasets (CSV and PostgreSQL)
  - 📄 real.csv: Dataset with register of product prices of 177 e-commerces in csv format.
  - 📄 synt.csv: Expanded dataset, ensuring that every retailers has every product in stock in csv format.
  - 📄 real.bak: Direct dump from the real dataset on PostgreSQL.
  - 📄 synt.bak: Direct dump from the synthetic dataset on PostgreSQL.
- 📂 **experiments**: Output files such as images and CSVs 
- 📂 **tests**: The files used as inputs of the recorded experiments. 




