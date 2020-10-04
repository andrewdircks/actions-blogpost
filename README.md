Supporting code for "Automate unit testing with Github Actions for research codes" waterprogramming blog. https://waterprogramming.wordpress.com/2020/10/05/automate-unit-testing-with-github-actions-for-research-codes/

# lake/
Includes two implementations of the Lake Model DPS formulation (Quinn et al. 2017)
- `lakemodel.py` is the standard implementation
- `lakemodel_fast.py` is the Numba optimized version

# Tests
- `test.py` executes unit tests on the standard lake model
- `test_fast.py` compares the results on random input for each implementation

# .github/workflows
- `test.yml` defines an Action for executing `test.py` with the `pytest` module
- `compare.yml` defines an Action for executing `test_fast.py` with the `pytest` module
