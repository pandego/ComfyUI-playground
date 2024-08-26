# ComfyUI Playground

Welcome to **ComfyUI-Playground** — a sandbox environment designed to facilitate the seamless use and exploration of ComfyUI. This repository provides a setup guide, pre-configured tools, and example workflows to help you get started quickly.

## 🚀 Quick Start

Follow these steps to clone the repository, set up the environment, and start using ComfyUI:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/pandego/ComfyUI-playground.git
   cd ComfyUI-playground
   ```

2. **Set Up the Environment:**

   Create the conda environment with all necessary dependencies:

   ```bash
   conda env create -f environment.yml
   conda activate comfyui
   ```

3. **Install Dependencies:**

   Use Poetry to install additional dependencies:

   ```bash
   poetry install --no-root
   ```

4. **Clone ComfyUI:**

   Clone the ComfyUI repository directly into your playground:

   ```bash
   git clone https://github.com/comfyanonymous/ComfyUI.git
   ```

5. **Install ComfyUI Manager and Additional Tools:**

   Set up the custom nodes and additional tools:

   ```bash
   cd ComfyUI/custom_nodes/
   git clone https://github.com/ltdrdata/ComfyUI-Manager.git
   cd ..
   ```

6. **Run ComfyUI:**

   Check available arguments:

   ```bash
   python main.py --help
   ```

   Start ComfyUI:

   ```bash
   python main.py
   ```
   
7. **Optional - Copy the Workflows to the `default/` folder:**

   There are a few Worflow examples in `workflows/` that you can copy to the ComfyUI's `default/` folder, like so:

   ```bash
   cp -r ../workflows/ user/default/
   ```

   They should now appear at the `default/`folder once you relaunch the ComfyUI.

## 📦 ComfyUI Manager and Additional Tools

This playground can then be supplemented with a variety of tools to enhance your ComfyUI experience. I will go for the following, and they can be added them directly through the [ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager):

- **[ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager):** Manage your ComfyUI configurations and workflows with ease.
- **[x-flux-comfyui](https://github.com/XLabs-AI/x-flux-comfyui):** Integrate advanced functionalities into your workflows.
- **[ComfyUI's ControlNet Auxiliary Preprocessors](https://github.com/Fannovel16/comfyui_controlnet_aux):** Utilize ControlNet features for enhanced control over your UI elements.
- **[SaveAsScript](https://github.com/atmaranto/ComfyUI-SaveAsScript):** Save your workflows as scripts for easy reuse and modification.

You can also check several tutos available online. I find this one from [stable-diffusion-art.com](https://stable-diffusion-art.com/comfyui/) to be a good start.

## 📁 Important Folders

Here are some key directories that you’ll be working with:

- **custom_nodes/x-flux-comfyui/workflows/:** Contains example workflows to help you get started.
- **user/default/workflows/:** This is where your saved workflows will be stored.
- **models/:** Organized by model types for easy access:
  - **models/clip/:** Text encoders. Check this for [FLUX.1](https://huggingface.co/comfyanonymous/flux_text_encoders/tree/main)
  - **models/clip_vision/:** Vision-based models for enhanced UI interactions.
  - **models/controlnet/:** ControlNet models for text-to-image transformations.
  - **models/vae/:** Variational Autoencoders (VAEs) for data compression and reconstruction tasks.

## 🤝 Contributing

Contributions are welcome! If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

## 📄 Acknowledgments

Special thanks to the developers of [ComfyUI](https://github.com/comfyanonymous/ComfyUI) and other contributors for providing the tools and inspiration to build this playground.

---

_Et Voilà !_ 🎈
