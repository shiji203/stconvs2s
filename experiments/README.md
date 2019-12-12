The `/experiments` folder has jupyter notebooks with the results of the first round of experiments. We conduct experiments with distinct numbers of layers, filters, and kernel sizes to investigate the best hyperparameters to fit the deep learning models. 

## Usage

**These notebooks are parameterized**. Therefore, to run it again use the following commands:

```
cd experiments
./run-notebooks.sh

```

When you run `run-notebook.sh` without parameter, it runs experiment experiments with default values. This script injects the settings defined in `dataset-variables.py` into the `base-stconvs2s.ipynb` (or `base-convlstm.ipynb`) and at the end generates a new notebook with the results.


### Positional Parameters

[1] `--stconvs2s` or `--convlstm`: change the model. Default model: stconvs2s
[2] `--cfsr` or `--chirps`: change the dataset to rainfall (CHIRPS). Default dataset: temperature (CFSR)