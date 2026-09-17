# Genetic Algorithm & Particle Swarm Optimization

What happens when two different population-based optimization algorithms explore the same landscape?

This project implements **Genetic Algorithm (GA)** and **Particle Swarm Optimization (PSO)** and experiments with their behavior on a collection of mathematical optimization problems.

The algorithms are tested on both **unimodal** and **multimodal** benchmark functions, making it possible to observe how different optimization landscapes affect their search.

## Algorithms

### Genetic Algorithm

- Selection
- Crossover
- Mutation
- Replacement

### Particle Swarm Optimization

- Particle positions and velocities
- Personal best (`pbest`)
- Global best (`gbest`)
- Boundary handling

## Benchmark Functions

The benchmark functions used in this project are based on the collection provided by [BenchmarkFcns](https://benchmarkfcns.info/fcns), which documents a variety of commonly used optimization test functions.

Some of the functions included are:

- Ackley
- Beale
- Booth
- Griewank
- Himmelblau
- Rastrigin
- Rosenbrock
- Schwefel
- Sphere
- Zakharov

## Running the Project

Install the required dependencies:

    pip install numpy pandas

Run the experiments with:

    python test.py

Running `test.py` executes the experiments and generates the result CSV files in the `results/` directory.

The `main.py` file contains the main project entry point and algorithm setup.

## Results

The generated results include:

- Average fitness
- Standard deviation
- Performance across benchmark functions
- Distance from the known global minimum

Results are organized into **unimodal** and **multimodal** functions.

## Project Structure

    .
    ├── algorithms/
    │   ├── benchmark.py
    │   ├── genetic_algorithm.py
    │   ├── pso_algorithm.py
    │   └── utility.py
    ├── docs/
    │   └── examples/
    ├── results/
    │   ├── multimodal_info.csv
    │   ├── multimodal_results.csv
    │   ├── unimodal_info.csv
    │   └── unimodal_results.csv
    ├── main.py
    └── test.py

## Reference

Benchmark functions:

[BenchmarkFcns](https://benchmarkfcns.info/fcns)

This project uses established benchmark functions to explore and compare the behavior of evolutionary and swarm-based optimization methods.
