# D4xC
A Distributed Circular Cross-Correlation Calculator

## Description

The circular cross-correlation is an important tool to detect similarities between two signals.
For two signals with n samples, x(k) and y(k), with 0 ≤ k < n, the circular cross-correlation rxy(τ) is defined by the formula:

<img src="https://github.com/FilipePires98/D4xC/blob/master/diagrams/formula.jpg" width="300px">

The goal of this project is to provide a fast calculator that reads in succession the values of pairs of signals stored in several data files, computes the circular cross-correlation of each pair and appends it to the corresponding file.
The source code contains three different implementations: one single-threaded, one multi-threaded and one resorting to the Message Passing Interface (MPI).

Notes: the project's dimension had to be reduced due to Covid-19 related constraints.

The execution times for the multithreaded version using a regular pc are:

<img src="https://github.com/FilipePires98/D4xC/blob/master/diagrams/tables/multithreaded-exectime-problem2.jpg" width="480px">

For the MPI version, the times are:

<img src="https://github.com/FilipePires98/D4xC/blob/master/diagrams/tables/mpi-exectime-problem2.jpg" width="440px">

## Repository Structure:

/dataset - contains the data files of the signals to be processed

/diagrams - contains visual representations of the program for analysis purposes

/src - contains the source code of all versions of the program

## Authors

The authors of this repository are Filipe Pires and João Alegria, and the project was developed for the Large Scale Computation Course of the Master's degree in Informatics Engineering of the University of Aveiro.

For further information, please contact us at filipesnetopires@ua.pt or joao.p@ua.pt.
