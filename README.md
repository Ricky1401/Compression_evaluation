# Compression_evaluation
This repository contains all the code about Rossetto Riccardo's thesis about how model compression techniques affect model bias

Run in this order:
- `ml-1m-statistics.ipynb`to generate the `TTE_uf--/TTE_user_split_uf--.json` file,
- `TTE_to_IO_dataset.ipynb` to generate `TTE_uf--/TTE_with_IO_uf--.json` and the train/test/eval splits,
- `PEFT` to generate the PEFT models and produce the base model processed file,

- `LA-Framework-quant/main.py quant` to quantize the model,
- `Gen-eval-quantized.ipynb` to generate quantized evaluation dataset,
  
- `LA-Framework-dist/main.py dist` to distil the model,
- `Gen-eval-distilled.ipynb` to generate distilled evaluation dataset,


- `Plot_on_eval_processed.ipynb` to compute metrics on generated data,