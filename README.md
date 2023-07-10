# Allele-genotype_Simulation
The code is a simulation of genetic inheritance and population dynamics. It explores how allele and genotype frequencies change over multiple reproductive cycles. The code is divided into two sections: a static model and a dynamic model.

Static Model:
- In the static model, the starting allele frequencies are defined for two alleles (T and M) using the variables `T_freq` and `M_freq`.
- Genotype frequencies are calculated based on the starting allele frequencies.
- The `simulate_offspring` function simulates the production of offspring based on the genotype frequencies of the parents. Offspring genotypes are randomly assigned according to the genotype frequencies.
- The `update_frequencies` function updates the allele and genotype frequencies based on the offspring produced.
- The `simulate_cycles` function simulates a given number of breeding cycles. It initializes the starting population of parents, and then iteratively simulates offspring production and frequency updates.
- The resulting allele and genotype frequencies are plotted over time using matplotlib.

Dynamic Model:
- The dynamic model extends the static model by introducing outcrossing between progeny.
- In this model, the starting genotype frequencies are defined for two parents using the variables `TT_freq`, `MM_freq`, and `MT_freq`.
- The `simulate_offspring` and `update_frequencies` functions are similar to the static model.
- The `simulate_cycles` function is modified to account for changes in allele frequencies due to outcrossing between progeny.
- The resulting allele and genotype frequencies are plotted over time using matplotlib.

By calling the `simulate_cycles` function with appropriate parameters (e.g., the number of starting pairs and the number of cycles), you can observe how allele and genotype frequencies change over time in the population.
