# GenAI Image Generator (Backend-Oriented)

This project is a backend-powered Generative AI application that generates
images from text prompts using Stable Diffusion.

## Architecture Overview

1. Configuration
   - Model name, device, inference parameters

2. Startup / Resource Initialization
   - Loads the Stable Diffusion model once at backend startup

3. Core Backend Logic
   - Handles request-time image generation using the preloaded model

4. Interface Layer
   - Gradio UI acting as a thin client

## Key Backend Concepts

- Long-lived resource management (model lifecycle)
- Separation of configuration, logic, and interface
- Backend service design (not a one-time script)
- GPU-backed inference using Stable Diffusion

## How to Run

1. Open the notebook in Google Colab
2. Enable GPU (Runtime → Change runtime type → GPU)
3. Run all cells
4. Enter a text prompt in the UI to generate an image

## Technologies

- Python
- Stable Diffusion
- Hugging Face Diffusers
- PyTorch
- Gradio
- Google Colab (GPU)
