# MinFit


This project consists of an R script for fitting bacterial growth rates to enzyme kinetic data. The R file takes as an input bacterial growth rates stressed with the antibiotic minocycline and enzyme kinetic data from several <i>E coli</i> mutants that contain TetX, an enzyme that degrates tetracycline type antibiotics. 

The script finds fit values the unknown parameters of a mathematical model for fitness to predict growth rates using the enzyme kinetic data. A monte-carlo method is used to determine the appropriate starting conditions to prevent false optimization peaks.

Robustness is tested by using a bootstrap method where each mutants is sequentially set aside and values are fit using the remaining mutants, and then the predicted growth rate for the mutant that has been set aside is calculated and compared to the known value.

