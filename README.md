# Clarity AI node for ComfyUI

This is a ComfyUI node for Clarity AI, the creative image upscaler. It upscales and enhances images to high resolution.

![alt text](dog_example.png)

## Free Usage:

We now have a fully ComfyUI workflow of Clarity upscaler, it seems to uses the same tech and is getting close to the clarity results. Needs some final tweaking to reach the same quality.
Feel free to experiment and let me know if you discover great parameters.

### 1. Install offline

Just drag and drop the `free-workflow.json` workflow json file into your ComfyUI.

You will need the ComfyUI-Manager to install the missing nodes.

Also you will need to install the following checkpoints:
* the tiling diffusion ControlNet: https://huggingface.co/copybaiter/ControlNet/blob/main/control_v11f1e_sd15_tile.safetensors
* a SD1.5 model (or the faster SD1.5-Hyper models)
* the two following LoRAs:
    * [SDXLrender v2](https://civitai.com/models/171159/sdxlrender)
    * [more details](https://civitai.com/models/82098/add-more-details-detail-enhancer-tweaker-lora)
* optionally, the upscaler: https://huggingface.co/datasets/jibopabo/upscalers/blob/main/4xNomosUniDAT_otf.pth

## Simple but paid usage:

### 1. Install Clarity AI node

Open ComfyUI Manager, search for Clarity AI, and install the node.

Alternatively:

```bash
cd custom_nodes
git clone https://github.com/philz1337x/ComfyUI-ClarityAI
```

### 2. Create your API key

Create an API key at: https://clarityai.cc/comfyui

### 3. Add the key to the node

Add the API key to the environment variable "`CAI_API_KEY`"

Alternatively, you can write your API key to a "`cai_platform_key.txt`" text file in the ComfyUI-ClarityAI folder.

Not recommended: You can also use and/or override the above by entering your API key in the '`api_key_override`' field. But be careful to delete the api_key_override when sharing your workflow.

<!--
A) Drag and drop this image, with the workflow inside, into ComfyUI and install missing nodes. -->
<!-- ![alt text](workflow_inside.png) -->
