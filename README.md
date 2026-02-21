# Compression_evaluation
This repository contains all the code about Rossetto Riccardo's thesis about how model compression techniques affect model bias

Run in this order:
- `ml-1m-statistics.ipynb`to generate the `TTE_uf--/TTE_user_split_uf--.json` file,
- `TTE_to_IO_dataset.ipynb` to generate `TTE_uf--/TTE_with_IO_uf--.json` and the train/test/eval splits,
- `PEFT` to generate the PEFT models and produce the base model processed file,
- `Plot_on_eval_processed.ipynb` to compute metrics on generate data,
- 
