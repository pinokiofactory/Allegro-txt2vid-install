# Allegro-txt2vid-pinokio
A Pinokio Install Script for the [Rhymes Allegro](https://github.com/rhymes-ai/Allegro) text-to-video model.


## NEWS
* Text+Img2vid is out!  It adds an extra pre-inference phase that spikes over 30GB VRAM. This extra phase takes an extra ~30 minutes on a 3090
* More info in the "Helpful Docs" accordion in the UI

## Sources
* Installs a Pinokio fork: https://github.com/pinokiofactory/Allegro-txt2vid
* Gradio UI and associated code borrowed from: https://huggingface.co/spaces/fffiloni/allegro-text2video
* RIFE Interpolation Model from [AlexWortega/RIFE](https://huggingface.co/AlexWortega/RIFE)

## Important Notes
* Can take over an hour to generate a result. Hopefully will be optimized soon. But yeah, 1 hour on a 3090.  4090 ~30 minutes. 
* 12GB VRAM should be sufficient to run, although it does briefly spike high in a couple of places, so make sure you haven't disabled SYSMEM fallback. 
* After the inference Steps have completed, there's a vae decode phase that can take quite a while. So don't panic and stop it prematurely!




```bibtex
@article{allegro2024,
    title={Allegro: Open the Black Box of Commercial-Level Video Generation Model},
    author={Yuan Zhou and Qiuyue Wang and Yuxuan Cai and Huan Yang},
    journal={arXiv preprint arXiv:2410.15458},
    year={2024}
}
