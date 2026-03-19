<div align="center">

  <img width="300" alt="MIPPIA Logo" src="https://github.com/user-attachments/assets/bc77c131-f5ee-449d-a438-60838917906a" />

  <br>

  <h1>🎵 AI-Generated Music Detection</h1>
  <h3>Fusion Segment Transformer: Bi-Directional Attention Guided Fusion Network for <br> AI-generated Music Detection</h3>

  <br>

  <p>
    <b>Yumin Kim*</b> • <b>Seonghyeon Go*</b>
  </p>
  <p>
    <b>MIPPIA Inc.</b>
  </p>

  <br>

  [![arxiv](https://img.shields.io/badge/arxiv-2601.13647-green)](https://arxiv.org/abs/2601.13647)
  [![Project Page](https://img.shields.io/badge/Project-Website-blue)](https://mippia.github.io/icassp-fst/)
  [![Demo Page](https://img.shields.io/badge/Demo-Page-red)](https://huggingface.co/spaces/mippia/AI-Music-Detection-FST)

</div>

<img width="2243" height="651" alt="Image" src="https://github.com/user-attachments/assets/9d08ef5f-cffc-4310-9537-de9e5a06600e" />

Official PyTorch implementation of **Fusion Segment Transformer (FST)** for **AI-generated music detection**.
This repository contains code and pretrained models for detecting AI-generated music audio.

Keywords: AI music detection, AIGM, music deepfake detection, Deepfake music

## Abstract
With the rise of generative AI technology, anyone can now easily create and deploy AI-generated music, which has heightened the need for technical solutions to address copyright and ownership issues. While existing works have largely focused on short-audio, the challenge of full-audio detection, which requires modeling long-term structure and context, remains insufficiently explored. To address this, we propose an improved version of the Segment Transformer, termed Fusion Segment Transformer. As in our previous work, we extract content embeddings from short music segments using diverse feature extractors. Furthermore, we enhance the architecture for full-audio AI-generated music detection by introducing a Gated Fusion Layer that effectively integrates content and structural information, enabling the capture of long-term context. Experiments on the SONICS and AIME datasets show that our approach consistently outperforms the previous model and recent baselines, achieving state-of-the-art results in full-audio segment detection. 

## 📖 Contents
  - [Installation](#installation)
  - [Requirements](#requirements)
  - [Download Checkpoints and Datasets](#download-checkpoints-and-datasets)
  - [Usage Inference](#usage-inference)
  - [License](#license)


## Installation

This repository can be installed simply by cloning the GitHub repository and installing the required dependencies.

```bash
git clone https://github.com/Mippia/FST-AI-music-detection.git
cd FST-AI-music-detection
```


## Requirements
To set up their environment, please run:
```bash
pip install -r requirements.txt
```

## Download Checkpoints and Datasets
To get started, download the our pre-trained checkpoints from Google Drive:
- [Stage-1 (MERT-AudioCAT)](https://drive.google.com/file/d/1frT4Mn0l6rso407Sy3eWCKbZmgwuVceN/view?usp=sharing)
- [Stage-2 (Fusion Segment Transformer)](https://drive.google.com/file/d/1E_xPsosYWI4UjKT8XQCbZW4ILvsWnmda/view?usp=sharing)


## Usage Inference
Use the inference.py script to check if music is AI-generated or human-made. For example,

```bash
python inference.py --audio ./examples/test.wav
```

## License
Our code and demo website are licensed under a 
  <a href="https://www.gnu.org/licenses/gpl-3.0.html" 
     class="text-blue-500 hover:underline">
    GPL License
  </a>.
