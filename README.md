# Looped Transformers

Few experiments with looped transformers. Code is based on `leiay/looped_transformer`.

Report with experiments:

https://api.wandb.ai/links/kkorolev/xnortnip

## Setup
Please install and activate the environment through
```shell
conda env create -f environment.yml
conda activate loop_tf
```

## Running Experiments
- For standard transformer training, refer to and execute  `bash exec/script_baseline.sh`.
- For looped transformer training, refer to and execute `bash exec/script_loop.sh`.
  - The parameter `b` determines the maximum loop iteration during training.
  - The parameter `T` sets the loop window size.
- To probe a trained model, refer to and execute `bash exec/script_probe.sh`.
- To work with the OpenML dataset for both standard and looped transformers, refer to and execute `bash exec/script_openml.sh`.
- To plot and compare with baseline methods, refer to notebooks in the `jupyter_notebooks` folder.
