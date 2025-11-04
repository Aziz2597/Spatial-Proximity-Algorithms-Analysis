# Spatial-Proximity-Algorithms-Analysis

## Project Overview

This project implements and empirically compares two algorithms for solving the Closest Pair of Points problem: a Brute Force approach (Θ(n²)) and a Divide & Conquer approach (Θ(n log n)). The analysis validates theoretical runtime predictions against empirical performance across large-scale inputs.

## Problem Significance

The Closest Pair of Points problem is fundamental in computational geometry with critical real-world applications:

- **Geographic Information Systems**: Finding nearest facilities, collision detection in spatial databases
- **Computer Vision**: Object recognition, feature matching in image processing
- **Network Design**: Optimal placement of network nodes or cellular towers
- **Data Mining**: Cluster analysis and anomaly detection in high-dimensional data
- **Robotics**: Path planning and obstacle avoidance systems
- **Bioinformatics**: Molecular structure analysis and protein folding

## Technical Implementation

### Algorithms

**Brute Force (ALG1)**
- Examines all pairwise combinations
- Guaranteed correctness through exhaustive search
- Time Complexity: Θ(n²)
- Space Complexity: Θ(1)

**Divide & Conquer (ALG2)**
- Recursively partitions problem space
- Combines solutions with efficient strip checking
- Time Complexity: Θ(n log n)  
- Space Complexity: Θ(n)

### Experimental Methodology

- **Scale**: Tested on inputs from 10,000 to 55,000 points
- **Rigor**: 10 iterations per input size with statistical averaging
- **Validation**: Cross-algorithm verification on identical inputs
- **Precision**: Millisecond timing with floating-point tolerance validation

## Key Results

### Performance Characteristics
- **Crossover Point**: Divide & Conquer outperforms Brute Force at ~10,000 points
- **Scalability**: Θ(n log n) algorithm maintains practical performance at scale
- **Constants**: Estimated hidden constants for runtime prediction:
  - Brute Force: c₁ = 2.8013 × 10⁻⁴
  - Divide & Conquer: c₂ = 8.0240 × 10⁻⁴

### Empirical Validation
- Theoretical complexity models confirmed through systematic measurement
- Algorithm correctness verified across diverse point distributions
- Practical limits of brute-force approach quantitatively demonstrated

## Technical Architecture

### Core Components
