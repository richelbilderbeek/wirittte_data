# wirittte_data

Data produced by WIRITTTES and analysed by WIRITTTEA.

## Usage

Use the scripts in the `demo` folder of [the WIRITTTEA GitHub](https://github.com/richelbilderbeek/wiritttea). 

Most scripts can be called in the following name:

```
[name].R [data folder] [output filename]
[name].sh [data folder] [output filename]
```

These three examples all do exactly the same:

Use R:

```
Rscript analyse_n_taxa.R ~/GitHubs/wiririttte_data/20170710 ~/n_taxa_20170710.csv
```

Use bash script:

```
./analyse_n_taxa.sh ~/GitHubs/wiririttte_data/20170710 ~/n_taxa_20170710.csv
```

On Peregrinne HPC:

```
sbatch analyse_n_taxa.sh ~/GitHubs/wiririttte_data/20170710 ~/n_taxa_20170710.csv
```

## Datasets

 * `20170710`: mutation rate = 0.01 (see [parameters_20170710.csv](parameters_20170710.csv) for all parameters used)

## FAQs

### Why only 960 data points?

Because the HPC cluster does not allow for more than 1000 jobs