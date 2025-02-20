# VLMs and Their Ability to Understand Meme's

This project demonstrates how to use Vision Language Models (VLMs) to understand and analyze memes using FiftyOne, Janus-Pro, and Moondream2. We explore different capabilities including OCR, meme understanding, and meme caption generation.

The idea for this project occured when the Janus Pro model by DeepSeek AI dropped. I was reading through the paper and in my hyped frame of mind I thought I read the model excels in MEME Perception...in fact, what the paper actually said was the model excels in [MME Perception](https://arxiv.org/abs/2306.13394). 

However, it turns out that MME-perception measures against a total of 10 subtasks for the evaluation of the perception ability, from the perspectives of coarse-grained recognition, fine-grained recognition, and OCR...which actually isn't all that different than meme perception.

Anyways, the end result is this small project which I hope you find entertaining.

## 🚀 Features

- OCR (Optical Character Recognition) on memes
- Meme scene and context understanding
- AI-powered meme caption generation
- Integration with FiftyOne for data visualization and management

## 🛠️ Prerequisites

- Python 3.10
- FiftyOne
- FiftyOne Plugins:
  - [Moondream2](https://github.com/harpreetsahota204/moondream2-plugin)
  - [Janus-Pro](https://github.com/harpreetsahota204/janus-vqa-fiftyone)

## 📦 Installation

1. Install FiftyOne:
   ```bash
   pip install fiftyone
   ```

2. Download and install the required plugins:
   ```bash
   fiftyone plugins download https://github.com/harpreetsahota204/janus-vqa-fiftyone
   fiftyone plugins requirements @harpreetsahota/janus_vqa --install

   fiftyone plugins download https://github.com/harpreetsahota204/moondream2-plugin
   fiftyone plugins requirements @harpreetsahota/moondream2 --install
   ```

3. Set the required environment variable:
   ```bash
   export FIFTYONE_ALLOW_LEGACY_ORCHESTRATORS=true
   ```

## 📊 Datasets

The project uses two datasets:
- ML Memes Dataset: A collection of machine learning-related memes

The dataset is available on [Hugging Face](https://huggingface.co/datasets/harpreetsahota/memes-dataset).

## 🎯 Use Cases

1. **OCR**: Extract text from memes using both Janus-Pro and Moondream2

2. **Meme Understanding**: Analyze the scene, characters, and humor in memes

3. **Caption Generation**: Generate AI-powered captions for meme templates

## 🚀 Getting Started

Check out the Jupyter notebook `vlm_meme_understanding.ipynb` for a step-by-step guide on how to:

- Load and visualize the datasets

- Set up the VLM operators

- Perform OCR, meme understanding, and caption generation tasks

- Visualize results using FiftyOne's web interface


## 🙏 Acknowledgments

- [Scott Penberthy's ML Memes](https://scott.ai/2019-08-06-memeified-ng)
- FiftyOne team for the plugin framework
- Creators of Janus-Pro and Moondream2