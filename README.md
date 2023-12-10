# Genetic-Algorithm-CVRP
Using genetic algorithm for solving CVRP Problem

# Overview
This repository provides an implementation of a Genetic Algorithm (GA) for solving the Capacitated Vehicle Routing Problem (CVRP). The CVRP is a well-known combinatorial optimization problem that involves efficiently routing a fleet of vehicles to deliver goods to a set of customers while respecting capacity constraints and minimizing the overall transportation costs, such as minimizing travel distance.

## About Genetic Algorithm model
# Crossover and Mutation Operators
Ordered Crossover: The crossover mechanism employed in this GA is the Ordered Crossover method. This operator combines genetic material from parent routes to generate new offspring, maintaining the relative order of genes.

Scrambled Mutation: The mutation operator involves the Scrambled Mutation method. This operation perturbs a small portion of the offspring routes, ensuring the validity of the routes while introducing diversity.
Users have the flexibility to experiment with alternative crossover and mutation strategies by modifying the code in the "crossover" and "mutation" functions.

# Parents Selection
Random Selection: The current implementation adopts random selection for choosing parent routes. Parents are randomly selected from the current population for participation in the crossover process.
Users are encouraged to explore and implement their own strategies for parent selection. By adjusting the "selected" variable function, you can experiment with different parent selection methods that align with the characteristics of your CVRP instances.

# Data used
Option 1 (Provided Data): Add the provided CVRP data from "CVRP Data.xlsx" to your environment.

Option 2 (Custom Data): Add your own CVRP data. Ensure it is a pd.DataFrame with the index 0 representing the depot location and demand. The DataFrame columns should be named 'X', 'Y', and 'Demand', providing the X and Y coordinates of each location and their corresponding demand.
