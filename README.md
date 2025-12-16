# A guide to using Nunchaku for SDXL models quantized using SVDQuant in Comfyui

## Prerequisites
1. Nunchaku for ComfyUI is properly installed and confirmed to work: https://github.com/nunchaku-tech/ComfyUI-nunchaku
2. Git is installed.

## Steps
1. Download a SDXL model that has been converted to SVDQuant. Make sure to get either the INT4 or FP4 according to your GPU architecture.
2. Start a terminal within the folder for the ComfyUI Nunchaku custom nodes (e.g. "ComfyUI/custom_nodes/ComfyUI-nunchaku").
     - For Windows 11, you can right click inside the folder and select "Open in Terminal"
3. Run this command to obtain the code that adds nodes for SDXL support: `git fetch origin pull/680/head:sdxlsupport`
     - The actual PR is at this link if you want to inspect the write-up or code: https://github.com/nunchaku-tech/ComfyUI-nunchaku/pull/680
4. Run this command to apply the changes to the current install: `git checkout sdxlsupport`
5. After launching ComfyUI, the SDXL nodes for model loading and LORA loading should be next to the other Nunchaku nodes.
