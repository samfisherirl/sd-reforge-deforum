# Don't Skip

You'll need to go to the 'extension' folder in /my_sd_reforge/webui/. Right click on the extensions folder, and uncheck read only. then click okay. This allows controlnet extension to be accessed from deforum. 

Moreover, to download controlnet, I downloaded it in forge, because I was testing both. Then copied the folder to the reforge location. You need to uncheck readonly after this step. 

found this fix looking to setup controlnet for deforum on reforge 

https://github.com/deforum-art/sd-webui-deforum/issues/949#issuecomment-1975278527


below is previous readme

# Deforum Stable Diffusion — official extension for Forge

This is the Deforum extension for the [Stable Diffusion WebUI Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge).
It is a fork of [the Deforum Extension for A1111](https://github.com/deforum-art/sd-webui-deforum) and is expected to diverge over time.

## Current status

This extension is **experimental**. It should load and basic settings should work. However, the full surface area of Deforum has not yet been tested. 
You are encouraged to take it for a spin and [raise issues here](https://github.com/deforum-art/sd-forge-deforum/issues) as you find problems.

## Installation

After setting up the [Stable Diffusion WebUI Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge):

    cd <forge_install_dir>/extensions
    git clone https://github.com/deforum-art/sd-forge-deforum
    cd sd-forge-deforum
    pip install -r requirements.txt

## What works & what doesn't

TODO

## Compatibility notes

* If you load a settings file from the a1111 extension into the Forge extension, you will need to reselect your controlnet preprocessors (they are referenced using different identifiers).
* Forge reduces VRAM usage by more agressively unloading models from memory. This can cause delays between frame generations while models are juggled in and of memory. To reduce this, start Forge with `--always-high-vram` (assuming you have sufficient VRAM).
