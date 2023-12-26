# mlx-explore/mlx-examples's llama.py with token/s timings and benchmarking-defaults

***This is based on [mlx-explore / mlx-examples/llm/llama](https://github.com/ml-explore/mlx-examples.git). Please consult its [README.md](https://github.com/ml-explore/mlx-examples/blob/main/README.md) for setup information.***

`llama_perf.py` is based on the original `llama.py` and prints additional timings. In order to compare MLX llama-2 inference performance (fp16 and quantized - use corresponding models) with [llama.cpp](https://github.com/ggerganov/llama.cpp/tree/master). Default is to run a 512 token prompt (to stress the GPUs), with a 128 token response, at temperature 0.0.

Note: it's inspired by the [llama.cpp Apple Silicon Benchmark Results](https://github.com/ggerganov/llama.cpp/discussions/4167)
