# Hardware notes

## Test machine

- GPU: GTX 1660 Super 6GB
- RAM: 16GB
- OS: Windows

## Main limitations

### VRAM
The biggest limitation is VRAM, especially for:
- larger models
- higher context
- fast generation
- agent/tool workflows with repeated calls

### System RAM
System RAM also matters when offloading is limited or when using CPU-heavy inference paths.

### Windows overhead
Windows setups can work well, but many guides assume Linux and skip practical Windows-specific issues.

## Practical lesson

Low-end local LLM use is possible, but only when:
- the model size is realistic
- quantization is chosen carefully
- context expectations stay grounded
- the user accepts tradeoffs
