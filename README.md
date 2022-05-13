# Chaos Theory

This project contains examples of 

## Installation

```bash
# Check if python is installed
python --version

# Install pipenv
pip install --user pipenv

# Install packages in virtual environment
pipenv install
```

Start virtual environment:

```
pipenv shell
```

Open and run `.ipynb` files with `Jupyter` extension for VSCode or with `jupyter notebook` inside the virtual environment.


## Population and logistic map

The logistic map is a polynomial mapping (equivalently, recurrence relation) of degree 2, often cited as an archetypal example of how complex, chaotic behaviour can arise from very simple non-linear dynamical equations. The map was popularized in a 1976 paper by the biologist Robert May, in part as a discrete-time demographic model analogous to the logistic equation written down by Pierre François Verhulst. Mathematically, the logistic map is written

`x[n+1] = r x[n] (1 - x[n])`

where `x[n]` is a number between zero and one, that represents the ratio of existing population to the maximum possible population. This nonlinear difference equation is intended to capture two effects:

* `reproduction` where the population will increase at a rate proportional to the current population when the population size is small.
* `starvation` (density-dependent mortality) where the growth rate will decrease at a rate proportional to the value obtained by taking the theoretical "carrying capacity" of the environment less the current population.

### References
* [The logistic difference equation and the route to chaotic behaviour](https://ethz.ch/content/dam/ethz/special-interest/usys/ibz/theoreticalbiology/education/learningmaterials/701-1424-00L/lde.pdf)
* [Ecology and Evolution: Populations](https://ethz.ch/content/dam/ethz/special-interest/usys/ibz/theoreticalbiology/education/learningmaterials/701-1424-00L/lecture-script-eep_2011.pdf)
* [Logistic map - Wikipedia](https://en.wikipedia.org/wiki/Logistic_map)
* [This equation will change how you see the world (the logistic map) - Veritasium](https://www.youtube.com/watch?v=ovJcsL7vyrk&ab_channel=Veritasium)

### Next steps
* Find if population has two convergence points (permanent oscillations between two values)
* Reduce growth rate step when convergence is not met
* Save and load calculations
* Plot on Matlab
* Animations