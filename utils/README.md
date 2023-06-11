# Running LLAMA

## Download LLAMA weights
Run `download_llama.sh` copied from this [link](https://github.com/shawwn/llama-dl) to get the weights.

## Convert LLAMA weights to HuggingFace

Run `python3 convert_llama_weights_to_hf.py 
    --input_dir /path/to/downloaded/llama/weights --model_size 7B --output_dir /output/path` from this huggingface [repo]( https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/convert_llama_weights_to_hf.py) to get the weights in huggingface format


## Sanity Check with MMLU 
Run `python3 run_mmlu_llama.py --ckpt_dir ~/llms/llama_hf/7B  --param_size 7` from [here](https://github.com/FranxYao/chain-of-thought-hub/tree/main/MMLU). 
Note, you still might get OOM issues. 
