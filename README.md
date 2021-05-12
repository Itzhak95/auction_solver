# Discrete auction solver

## Running the code 

Running the code is simple:
* Download the code from GitHub.
* Make sure that Python is installed on your machine.
* Install the required modules.
* Run the file main.py.

When you run the file main.py, you should be prompted to supply various pieces of information (e.g. the number of bidders in your auction).

## Viewing the equilibrium

The equilibrium constructed by the algorithm is recorded in the Excel file results.xlsl (which you should have downloaded with the code). The table should be self-explanatory:
* The first column lists every possible value that a player could have (these are integers starting from 0).
* The second column specifies the bids that are bid with positive probability (in equilibrium) by a player with that particular value. For instance, an entry of [0, 1, 2] means that the equilibrium bids (at that value) are 0, 1 and 2.
* The third column specifies the probabilities with which the equilibrium bids are submitted.
* If values are uniformly distributed, there is also a fourth column which records the predictions of an 'analogous' continuous model. In the 'analogous' model, bids can be any real number (not just integers); and values are are drawn from a continuous uniform distribution on [0, x] where x is the maximum possible value (which you yourself will have specified when running the code).

After constructing the equilibrium, the program then checks (by direct calculation) that it is indeed an equilibrium. The result of this check is printed in the terminal.
