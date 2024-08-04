# Direct Addressing GQA

This repository implements **Direct Addressing GQA** to optimize memory usage in Transformer models by avoiding the doubling of memory requirements for key-value (KV) pairs caused by `repeat_kv`.

This approach is based on Triton's fused attention tutorial.

## Features

- **Memory Efficiency**: Reduces KV memory requirements with direct addressing.
- **Fused Attention**: Utilizes Triton's fused attention for improved performance.

## TODO
- [ ] support N_CTX < 128, pls note current model only works for N_CTX = 128 * int(). That's because of the bug in fused-attention tutorial. You can choose right padding to 128 * int() to avoid such bug.
