# AMD ROCm LLM Inference Optimization

High-performance Large Language Model inference on AMD MI300X GPUs using ROCm, PyTorch, and vLLM.

## 🎯 Project Goals

- Optimize LLM inference performance on AMD MI300X architecture
- Benchmark PyTorch vs vLLM inference throughput
- Implement quantization techniques (AWQ, GPTQ) for ROCm
- Build production-ready inference API with SGLang

## 🔧 Tech Stack

- **Hardware:** AMD MI300X (192GB HBM3, 153B transistors)
- **Software:** ROCm 6.4.0, PyTorch 2.5+, vLLM, SGLang
- **Models:** Llama 3.1 70B, Mixtral 8x22B, Qwen2.5 72B

## 📊 Performance Targets

- Llama 3.1 70B: >50 tokens/sec (BF16)
- Mixtral 8x22B: >30 tokens/sec (AWQ 4-bit)
- Multi-GPU scaling efficiency: >85%

## 🚀 Roadmap

- [x] Environment setup (ROCm 6.4.0 + PyTorch)
- [ ] Baseline benchmarks (PyTorch native)
- [ ] vLLM integration and optimization
- [ ] Quantization experiments (AWQ/GPTQ)
- [ ] Multi-GPU distributed inference
- [ ] Production API deployment (SGLang + FastAPI)

## 📝 Requirements

```
rocm==6.4.0
torch==2.5.0+rocm6.1
vllm>=0.6.0
transformers>=4.45.0
accelerate>=0.34.0
```

## 🤝 Contributing

Open to collaboration on ROCm optimization techniques and benchmark results.

## 📄 License

MIT License - see LICENSE file for details.

## 🔗 Resources

- [AMD ROCm Documentation](https://rocm.docs.amd.com/)
- [vLLM on ROCm](https://docs.vllm.ai/en/latest/getting_started/amd-installation.html)
- [MI300X Whitepaper](https://www.amd.com/en/products/accelerators/instinct/mi300.html)
