# SmolVLM real-time camera demo

![demo](./demo.png)

This repository is a fork of the [simple demo](https://github.com/ngxson/smolvlm-realtime-webcam) for how to use llama.cpp server with SmolVLM 500M to get real-time object detection.

Based on the upstream code, this repository adds the capability to optionally specify the LLM API key and model name, allowing the demo to work not only with the original `llama.cpp` but also with [Ollama](https://github.com/ollama/ollama/) together with [litellm proxy](https://github.com/BerriAI/litellm).

## How to setup

1. Install [llama.cpp](https://github.com/ggml-org/llama.cpp)
2. Run `llama-server -hf ggml-org/SmolVLM-500M-Instruct-GGUF`  
   Note: you may need to add `-ngl 99` to enable GPU (if you are using NVidia/AMD/Intel GPU)  
   Note (2): You can also try other models [here](https://github.com/ggml-org/llama.cpp/blob/master/docs/multimodal.md)
3. Open `index.html`
4. Optionally change the instruction (for example, make it returns JSON)
5. Click on "Start" and enjoy
