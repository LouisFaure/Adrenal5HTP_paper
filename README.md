# Adrenal5HTP

Raw and processed data is available on the following GEO Series:
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180861

## Environment setup

```bash
conda create -n 5HTP -c anaconda python=3.9 -y
conda activate 5HTP
pip install brie==2.0.5 scanpy scFates
```

### GPU (Optional)
BRIE code can be accelerated with CUDA GPU.
```bash
conda install -c anaconda cudatoolkit -y
pip install -U tensorflow-gpu
```


## Running the notebooks

1. [Process.ipynb](https://github.com/LouisFaure/Adrenal5HTP_paper/blob/main/Process.ipynb) scRNAseq data pre-processing, clustering and embedding generation.
2. [BRIE2.ipynb](https://github.com/LouisFaure/Adrenal5HTP_paper/blob/main/BRIE2.ipynb) running BRIE2 pipeline, requires BAM files generated from alignment.
3. [Plots.ipynb](https://github.com/LouisFaure/Adrenal5HTP_paper/blob/main/Plots.ipynb) to generate plots for the manuscript.
