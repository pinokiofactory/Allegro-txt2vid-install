# Allegro-txt2vid-pinokio
A Pinokio Install Script for the [Rhymes Allegro](https://github.com/rhymes-ai/Allegro) text-to-video model.

## Sources
* Installs a Pinokio fork: https://github.com/pinokiofactory/Allegro-txt2vid
* Gradio UI and associated code borrowed from: https://huggingface.co/spaces/fffiloni/allegro-text2video
* RIFE Interpolation Model from [AlexWortega/RIFE](https://huggingface.co/AlexWortega/RIFE)

## Important Notes
* Can take over an hour to generate a result. Hopefully will be optimized soon. But yeah, 1 hour on a 3090.  4090 ~30 minutes. 
* Could be technically runnable on AMD and Mac, but might take 10x longer... 
* My GPU warms me at night. 
* 12GB VRAM should be sufficient to run, although it does briefly spike high in a couple of places, so make sure you haven't disabled SYSMEM fallback. 
* After the inference Steps have completed, there's a vae decode phase that can take quite a while. So don't panic and stop it prematurely!


* Img2vid is in the works apparently: https://github.com/rhymes-ai/Allegro/issues/8
* Yes, it's not (yet) optimized for consumer GPUs: https://github.com/rhymes-ai/Allegro/issues/20


![2024-10-26 16-54-31](https://github.com/user-attachments/assets/d25878c1-a691-4b5b-b0a5-545a988f9450)


```bibtex
@article{allegro2024,
    title={Allegro: Open the Black Box of Commercial-Level Video Generation Model},
    author={Yuan Zhou and Qiuyue Wang and Yuxuan Cai and Huan Yang},
    journal={arXiv preprint arXiv:2410.15458},
    year={2024}
}
