# Snakemake bioinformatic workflow example

Install all required software:

```console
mamba env create --name snakemake-tutorial --file environment.yaml
```

Visualization of the DAG:

```console
snakemake --dag plots/quals.svg | dot -Tsvg > dag.svg
```

Run full workflow:

```console
snakemake --cores 1 plots/quals.svg
```