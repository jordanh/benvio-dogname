# Benign Violation Theory of Humor Dog/Name Experiment

Enclosed are the project source files and data to conduct
and analyze your very own dog/name juxtaposition experiment
to test the Benign Violation Theory of Humor.

Contained in this source repository are three sub-directories:

   1. `data/` – source word lists and experimental results
   2. `notebooks/` – iPython name generator and analysis source
   3. `mturk/` – Amazon Mechanical Turk HIT source


## Installation

In order to generate your own dog/name combinations and
analyze the results, you'll need iPython and several
statistical analysis and visualization packages installed
on your local machine.

You'll need to perform the following from the command-line:

### 1. Install pip

`$ sudo easy_install pip`

### 2. Install iPython with all the options:

`$ sudo pip install ipython[all]`

### 3. Install statistical and visualization modules:

`$ sudo pip install pandas numpy scipy matplotlib statsmodels seaborn`


## Usage

### Generating the dog/name combinations

   1. Run an iPython notebook: `$ ipython notebook`
   2. Within the notebook, open `notebooks/Dog Name Generator.ipynb`
   3. Run the notebook, names will be written to `output.csv`

### Administering the Experiment on Amazon Mechanical Turk

   1. Create an account at: https://www.mturk.com/mturk/welcome
   2. Navigate to the _Create_ tab
   3. Create a _New Project_
   4. Create an _Other_ project (custom)
   5. Title your project, set title and keywords as desired
   6. Set pricing
   7. Set number of assignments per HIT to desired replication
   8. Click on _Advanced »_ and select only native English speaking countries
   9. Click on the _Design Layout_ button and then the _Source_ button
   10. Paste in the desired experimental HTML from the `mturk/` directory
   11. Save the HIT
   12. Publish the batch using `output.csv` dog/name image combinations

### Analyzing the results

   1. Download the results from Amazon Mechanical Turk as a .csv
   2. Use Google Sheets or similar spreadsheet tools to generate a data table similar to `data/results-exp1.csv` or `data/results-exp2.csv`

      * For Experiment 1, see: https://docs.google.com/spreadsheets/d/1yfXAnT7SXehxbZ8x4GOw15H39RhQky9ZWf-JgBlrkBE/edit#gid=1964811542
      * For Experiment 2, see: https://docs.google.com/spreadsheets/d/1WMm7PNsLsV9afygzJp-Zw4buuTd96dj597lOo0mEdYM/edit#gid=1838149423

   3. Open the iPython notebook `notebooks/Statistical Analysis.ipynb`
   4. Run the notebook


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D


## License

This source and data are licensed under the GPLv3 free software license. See: http://www.gnu.org/licenses/gpl-3.0.html
