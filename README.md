# Direct Addressing GQA

This repository implements **Direct Addressing GQA** to optimize memory usage in Transformer models by avoiding the doubling of memory requirements for key-value (KV) pairs caused by `repeat_kv`.

This approach is based on Triton's fused attention tutorial.

## Features

- **Memory Efficiency**: Reduces KV memory requirements with direct addressing.
- **Fused Attention**: Utilizes Triton's fused attention for improved performance.
