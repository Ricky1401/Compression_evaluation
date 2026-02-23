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


Statistiche (su PEFT con output invertito):
- PEFT 90_2048 : 1h01
- Generation with PEFT 90_2048-batched-64 : 3h19
- Quantizing PEFT 90_2048 : 0h12
- Generation with quantized model batched-64 : 3h19

- PEFT 90_Qwen3-1.7B : 1h01
- Generation with PEFT 90_Qwen3-1.7B : 3h19
- Quantizing PEFT 90_Qwen3-1.7B : 0h7
- Generation with quantized model batched-64 : 1h45

Statistiche (su PEFT con output corretto):
- PEFT 90_2048 : 
- Generation with PEFT 90_2048-batched-64 : 
- Quantizing PEFT 90_2048 : 
- Generation with quantized model batched-64 : 

- PEFT 90_Qwen3-1.7B : 
- Generation with PEFT 90_Qwen3-1.7B : 
- Quantizing PEFT 90_Qwen3-1.7B : 
- Generation with quantized model batched-64 : 