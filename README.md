# mlx-explore/mlx-examples's `llama.py` and `mixtral.py` with token/s timings and better benchmarking-defaults

***This is based on [mlx-explore / mlx-examples/llm](https://github.com/ml-explore/mlx-examples.git). Please consult its [README.md](https://github.com/ml-explore/mlx-examples/blob/main/README.md) for setup,... information.***

Use the files with either a --model_dir argument or provide a linked mlx_model directory to it. In order to compare MLX llama-2 inference performance (fp16 and quantized - use corresponding models) with [llama.cpp](https://github.com/ggerganov/llama.cpp/tree/master). 

Default is to run a 512 token prompt (to stress the GPUs), with a 128 token response. Comparable to the [llama.cpp Apple Silicon Benchmark Results](https://github.com/ggerganov/llama.cpp/discussions/4167)

`llama_perf.py` is based on the original `llama.py` and prints additional timings - warning, its now based on an outdated llama.py and provided just for reproduceability of [my medium.com paper](https://medium.com/@andreask_75652/benchmarking-apples-mlx-vs-llama-cpp-bbbebdc18416).

`llama_timings.py` is based on the updated `llama.py` from 2024-12-27. Default is to run a 512 token prompt (to stress the GPUs), with a 128 token response. Please note that it's timing-split between prompt-processing and token-generation is off by one token.

`llama_timings.py` does the same for Mixtral models based on `mixtral.py` from 2024-12-27. Default is to run a 512 token prompt (to stress the GPUs), with a 128 token response.
