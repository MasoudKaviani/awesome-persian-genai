# Awesome Persian GenAI

A curated list of open-source Generative AI resources for Persian (Farsi) — including Large Language Models, embedding models, text-to-speech, speech recognition, text-to-image, OCR, datasets, and benchmarks.

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## Table of Contents

- [Large Language Models (LLMs)](#large-language-models-llms)
- [Specialized & Domain-Specific Models](#specialized--domain-specific-models)
- [Encoder & BERT-style Models](#encoder--bert-style-models)
- [Embedding Models](#embedding-models)
- [Text-to-Speech (TTS)](#text-to-speech-tts)
- [Speech Recognition (ASR / STT)](#speech-recognition-asr--stt)
- [Text-to-Image Generation](#text-to-image-generation)
- [Image Captioning & Vision-Language](#image-captioning--vision-language)
- [OCR Models](#ocr-models)
- [Tokenizers](#tokenizers)
- [Datasets](#datasets)
- [Benchmarks & Leaderboards](#benchmarks--leaderboards)
- [Tools & Frameworks](#tools--frameworks)

---

## Large Language Models (LLMs)

| Model | Link | Description |
|-------|------|-------------|
| Dorna-Llama3-8B | https://huggingface.co/PartAI/Dorna-Llama3-8B-Instruct | Fine-tuned Llama-3-8B on a large Persian instruction dataset by Part AI. Available in multiple GGUF quantizations for consumer hardware. |
| Dorna2-Llama3.1-8B-Instruct | https://huggingface.co/PartAI/Dorna2-Llama3.1-8B-Instruct | Updated Dorna model built on Llama-3.1-8B-Instruct. Achieved 50.72% average accuracy on five Persian tasks, outperforming Maral-7B and PersianMind-7B. |
| PersianMind | https://huggingface.co/universitytehran/PersianMind-v1.0 | Extends LLaMA-2-7B with 10,000 Persian tokens, trained on 2B Persian tokens by University of Tehran. Cross-lingual Persian-English, comparable to GPT-3.5-turbo in reading comprehension. Non-commercial license. |
| PersianLLaMA-13B | https://huggingface.co/ViraIntelligentDataMining/PersianLLaMA-13B | 13B parameter model trained on Persian Wikipedia for text generation and instruction tuning. |
| IbnSina-3b | https://huggingface.co/ibnsina-llm/ibnsina-3b | Pre-trained from scratch on Persian corpora plus a 2B synthetic STEM and reasoning dataset. Also available on Ollama. |
| IbnSina-1.5b | https://huggingface.co/ibnsina-llm/ibnsina-1.5b | Smaller variant of IbnSina, pre-trained from scratch for Persian. |
| Zagros-1.0-Quick | https://huggingface.co/darsadilab/zagros-1.0-quick | Mixture-of-Experts (MoE) model specialized for high-performance Persian NLP. |
| gemma-3n-E4B-persian | https://huggingface.co/mshojaei77/gemma-3n-E4B-persian | Persian fine-tune of Gemma-3n, optimized for conversational chat and instruction following in Farsi. |
| gemma3persian | https://huggingface.co/mshojaei77/gemma3persian | Persian fine-tuned Gemma 3 model for chat and instruction tasks. |
| Maral-7B-alpha-1 | https://huggingface.co/MaralGPT/Maral-7B-alpha-1 | Bilingual Persian-English model based on Mistral, trained with PEFT and QLoRA on a Persian translation of the Alpaca dataset. |
| Strawberry-1 | https://huggingface.co/artindnr/strawberry-1 | ~20B parameter model fine-tuned from openai/gpt-oss-20b for high-quality Farsi reasoning chains. Apache 2.0 license, commercial use allowed. |
| Blueberry-2 | https://huggingface.co/artindnr/BlueBerry-2 | 117B parameter bilingual Farsi-English model fine-tuned for code-switching and mixed-language reasoning. |
| Persian-Phi | https://huggingface.co/amirakhlaghiqqq/PersianPhi | 3.85B parameter model adapted from Microsoft Phi-3 Mini via tokenizer extension, embedding warm-up, and continual pre-training. Resource-efficient approach with competitive leaderboard results. |
| AVA-Mistral-7B | https://github.com/mehdihosseinimoghadam/AVA-Mistral-7B | Fine-tuned Mistral 7B Persian LLM (weights on Hugging Face). |
| AVA-Llama-3 | https://github.com/mehdihosseinimoghadam/AVA-Llama-3 | Fine-tuned Llama 3 Persian LLM (weights on Hugging Face). |
| AVA-Llama-3-V2 | https://huggingface.co/MehdiHosseiniMoghadam/AVA-Llama-3-V2 | Updated version of AVA-Llama-3 fine-tuned for Persian chat and instruction following. |
| AVA-Qwen1.5-7B-Chat | https://github.com/mehdihosseinimoghadam/AVA-Qwen1.5-7 | Fine-tuned Qwen1.5-7B Persian LLM for chat applications. |
| Hormoz 8B | https://github.com/Mann-E/hormoz | Multilingual on-device model with special support for Persian and Arabic, based on Command R. |
| tea-4bit | https://huggingface.co/artindnr/tea-4bit | 4-bit quantized multilingual Llama model fine-tuned for Persian and English chat and QA. |
| PersianSciQA-LLaMA-13B-GGUF | https://huggingface.co/mradermacher/PersianSciQA-LLaMA-13B-GGUF | GGUF-quantized version of PersianSciQA LLaMA-13B, specialized for scientific QA in Persian. |
| Persian-llm-fibonacci-1-7b-chat | https://huggingface.co/MohammadRostami/Persian-llm-fibonacci-1-7b-chat.P1_0 | 7B Persian chat model fine-tuned from Llama architecture. |
| fibonacci-2-9b | https://huggingface.co/fibonacciai/fibonacci-2-9b | 9.24B parameter model based on Gemma2 architecture. Available in multiple GGUF quantizations (4-bit to 16-bit). |
| fibonacci-2-14B | https://huggingface.co/fibonacciai/fibonacci-2-14B | 14B parameter model based on Phi 4 architecture, supporting Farsi among multiple languages. |
| mGPT-1.3B-persian | https://huggingface.co/ai-forever/mGPT-1.3B-persian | 1.3B parameter mGPT model further fine-tuned for Persian text generation. Resource-efficient proof-of-concept. |
| AriaGPT | https://huggingface.co/ViraIntelligentDataMining/AriaGPT | Persian GPT model trained on large-scale Persian text corpus. |
| laya-fa-support | https://huggingface.co/tarfandoon/laya-fa-support | Persian language support model for the Laya architecture. |
| Dibachain/Diba-Base | https://huggingface.co/Dibachain/Diba-Base | Persian base language model for general NLP tasks. |

---

## Specialized & Domain-Specific Models

| Model | Link | Description |
|-------|------|-------------|
| BioPars | https://huggingface.co/parsi-ai-nlpclass/BioPars | First comprehensive Persian biomedical LLM. Full pipeline from pre-training on biomedical corpora to instruction tuning. For medical question answering. |
| BERT-Persian-Poetry | https://huggingface.co/mitra-mir/BERT-Persian-Poetry | BERT model post-trained on extensive Persian poetry datasets (Ganjoor) for understanding and generating poetic text. |
| ALBERT-Persian-Poetry | https://huggingface.co/mitra-mir/ALBERT-Persian-Poetry | ALBERT model fine-tuned on Persian poetry for stylistic text generation and analysis. |
| llama_poetry_fa | https://huggingface.co/8lianno/llama_poetry_fa | Llama 3.1-based model fine-tuned for generating stylistically coherent and culturally resonant Persian poetry. |
| BaSalam/Llama2-7b-entity-attr-v1 | https://huggingface.co/BaSalam/Llama2-7b-entity-attr-v1 | Fine-tuned Llama-2-7B for generating structured Persian product catalogs in JSON. Trained on data from Iranian e-commerce platforms using LoRA. |
| RealRobot-Chatbot (E-commerce) | https://huggingface.co/fibonacciai/RealRobot-Chatbot-Ecommerce-Robot-Fibonacci-Nano-llm | GGUF model fine-tuned as a conversational e-commerce chatbot for Persian product inquiries. |
| Finetune_mBert_Persian_law | https://huggingface.co/SinaRp/Finetune_mBert_Persian_law_1 | Fine-tuned mBERT specifically trained for Persian legal analysis, clause extraction, and document summarization. |

---

## Encoder & BERT-style Models

| Model | Link | Description |
|-------|------|-------------|
| ParsBERT | https://huggingface.co/HooshvareLab/bert-fa-base-uncased | Monolingual Persian BERT pre-trained on large Persian corpora (3.9M+ documents). The foundational Persian encoder model. |
| ParsBERT (GitHub) | https://github.com/hooshvare/parsbert | Official repository with training scripts, datasets, and evaluation code for ParsBERT. |
| FaBERT | https://huggingface.co/sbunlp/fabert | Persian BERT-base model pre-trained on the HmBlogs corpus (informal and formal Persian). |
| AriaBERT | https://huggingface.co/ViraIntelligentDataMining/AriaBERT | Persian BERT model trained on 32GB+ of varied Persian text data. |
| ParsT5 | https://huggingface.co/persiannlp/mt5-large-parsinlu-opus-translation_fa_en | mT5 large model adapted for Persian translation and NLU tasks. |
| gpt2-persian | https://huggingface.co/bolbolzaban/gpt2-persian | GPT-2 model pre-trained from scratch on Persian text, originally developed for poetry generation research. |

---

## Embedding Models

| Model | Link | Description |
|-------|------|-------------|
| Hakim | https://huggingface.co/MCINext/Hakim | State-of-the-art Persian text embedding model, 8.5% improvement over previous approaches on FaMTEB. |
| heydariAI/persian-embeddings | https://huggingface.co/heydariAI/persian-embeddings | Fine-tuned XLM-RoBERTa for high-quality Persian sentence/paragraph embeddings. Supports semantic search, clustering, and similarity. |
| persian-embeddings-gguf | https://huggingface.co/alishendi/persian-embeddings-gguf | GGUF conversion of heydariAI/persian-embeddings for use with Ollama and llama.cpp. |
| heydariAI/persian-embeddings (Ollama) | https://ollama.com/aligh4699/heydariAI-persian-embeddings:latest | Persian sentence embedding model in GGUF format for Ollama. |

---

## Text-to-Speech (TTS)

| Model | Link | Description |
|-------|------|-------------|
| Mana-Persian-Piper | https://huggingface.co/MahtaFetrat/Mana-Persian-Piper | Persian Piper TTS fine-tuned on Mana-TTS, optimized for low-latency on-device inference. |
| ManaTTS-Persian-Tacotron2 | https://github.com/MahtaFetrat/ManaTTS-Persian-Tacotron2-Model | Tacotron2 Persian TTS trained on the largest open single-speaker Persian speech dataset (114+ hours). Weights on Hugging Face. |
| Persian-Tacotron2-on-ManaTTS | https://github.com/Adibian/Persian-TTS-Zoo | Tacotron2 model trained on ManaTTS dataset, released under CC0-1.0 license. Part of the Persian-TTS-Zoo collection. |
| persian-tts-male1-vits | https://github.com/karim23657/Persian-tts-coqui | Male-voice VITS model for Persian TTS using the Coqui framework. |
| pertts (Piper Persian TTS) | https://github.com/SadeghKrmi/pertts-streamlit | Web interface for Persian TTS powered by the Piper engine. Includes multiple AI voices trained on open-source datasets. |
| MOSS-TTS-Nano-Persian | https://huggingface.co/nimaaaAI/MOSS-TTS-Nano-Persian | Persian fine-tune of a compact 117M parameter TTS model, trained on 34,000 Persian clips. |
| Gooya-RizehPizeh-v2-exp | https://huggingface.co/Reza2kn/Gooya-RizehPizeh-v2-exp | Experimental Persian TTS model with verified offline CPU inference. |
| Chatterbox-TTS-Persian-Farsi | https://huggingface.co/Thomcles/Chatterbox-TTS-Persian-Farsi | TTS model trained on cleaned, denoised, transcribed and filtered Persian data. |
| pocket-tts-farsi-v2 | https://huggingface.co/mehdi-hf/pocket-tts-farsi-v2 | Compact Persian TTS model that reads Persian script directly without a grapheme-to-phoneme converter. Trained on ~497 hours of speech. |
| pocket-tts-farsi-v2-onnx | https://huggingface.co/Nimaone/pocket-tts-farsi-v2-onnx | ONNX export of pocket-tts-farsi for optimized inference. |
| mimic3 (Persian) | https://github.com/MycroftAI/mimic3 | Fast, local neural TTS system supporting Persian voices. |

---

## Speech Recognition (ASR / STT)

| Model | Link | Description |
|-------|------|-------------|
| BuzzASR/persian | https://huggingface.co/BuzzASR/persian | Monolingual Persian ASR model fine-tuned from openai/whisper-large-v3. |
| whisper-persian-v4 | https://huggingface.co/nezamisafa/whisper-persian-v4 | Fine-tuned openai/whisper-large-v3 on the ASR_fa_v1 dataset for Persian speech recognition. |
| whisper-persian (LoRA) | https://huggingface.co/Paulwalker4884/whisper-persian | Fine-tuned Whisper-base for Persian STT using LoRA, real-time capable. Handles various Persian accents and speaking styles. |
| whisper-large-fa-v1 | https://huggingface.co/vhdm/whisper-large-fa-v1 | Whisper large model fine-tuned for Persian Farsi transcription. |
| neyshekar-whisper-large-v3-lora | https://huggingface.co/hosseinzr/neyshekar-whisper-large-v3-lora | Whisper-large-v3 with LoRA fine-tuning for Persian speech recognition. |
| whisper-small-fa (hezar) | https://huggingface.co/hezarai/whisper-small-fa | Whisper-small fine-tuned for Persian ASR, integrated into the Hezar toolkit. |
| wav2vec2-large-xlsr-53-persian | https://huggingface.co/jonatasgrosman/wav2vec2-large-xlsr-53-persian | Wav2Vec2 XLSR-53 fine-tuned for Persian speech recognition. |
| wav2vec2-large-xlsr-persian (m3hrdadfi) | https://huggingface.co/m3hrdadfi/wav2vec2-large-xlsr-persian | Another Wav2Vec2 XLSR fine-tune for Persian ASR. |

---

## Text-to-Image Generation

| Model | Link | Description |
|-------|------|-------------|
| Jimage-L2 | https://huggingface.co/JibayAi/Jimage-L2 | Text-to-image system with full Persian and English support. |
| Jimage-L1 | https://huggingface.co/JibayAi/Jimage-L1 | Advanced text-to-image generator with Persian/English support and 63 built-in Persian fonts. |
| image-generation-mt5-finetune | https://huggingface.co/parsi-ai-nlpclass/image-generation-mt5-finetune | Pipeline that translates Persian text to English then generates images using a fine-tuned Stable Diffusion model. |
| persian-posters (LoRA) | https://huggingface.co/Mehrdadsb/persian-posters | LoRA adapter for FLUX.1-dev that generates Persian-style posters. Uses trigger word 'PSNPOSTERS' in prompts. |
| Iranian Actor Behroz Vosughi (LoRA) | https://huggingface.co/xail/Iranian_Actor_Behroz_Vosughi_Flux_LoRa | LoRA for FLUX trained on 13 images to generate artistic portraits of the Iranian actor Behroz Vosughi. |

---

## Image Captioning & Vision-Language

| Model | Link | Description |
|-------|------|-------------|
| Persian-Image-Captioning | https://huggingface.co/MahsaShahidi/Persian-Image-Captioning | Image captioning model that generates Persian descriptions from images. |
| Qwen3-VL-2B-Persian-Arabic-OCR | https://huggingface.co/mohajesmaeili/Qwen3-VL-2B-Persian-Arabic-Ocr-v1.0 | Vision-language model fine-tuned for Persian and Arabic OCR on 156K text line images. |

---

## OCR Models

| Model | Link | Description |
|-------|------|-------------|
| Persian_OCR | https://huggingface.co/WeightedAI/Persian_OCR | Trained on 600K synthetic Persian text images from Wikipedia with 49 Persian fonts. Achieves 96% sequence accuracy. |
| hezarai/crnn-base-fa-v2 | https://huggingface.co/hezarai/crnn-base-fa-v2 | CRNN-based Persian OCR model integrated into the Hezar AI toolkit. |
| Shenava-Koochik-v1.0 | https://huggingface.co/PersianML/Shenava-Koochik-v1.0 | Persian OCR model by PersianML community for document text recognition. |
| Shenava-RizehPizeh-v1.0 | https://huggingface.co/Reza2kn/Shenava-Rizeh-v1.0 | Persian text recognition model for fine-grained OCR tasks. |

---

## Tokenizers

| Model | Link | Description |
|-------|------|-------------|
| PersianBPETokenizer | https://huggingface.co/mshojaei77/PersianBPETokenizer | Custom BPE tokenizer specifically designed for the Persian (Farsi) language. |

---

## Datasets

| Dataset | Link | Description |
|-------|------|-------------|
| Mana-TTS Dataset | https://huggingface.co/datasets/MahtaFetrat/Mana-TTS-Dataset | Largest open single-speaker Persian speech dataset (114+ hours) for TTS training. CC0 license. |
| ParsVoice | https://huggingface.co/datasets/MohammadJRanjbar/ParsVoice | Largest publicly available multi-speaker Persian speech corpus (1,800+ hours) for TTS training, with zero-shot cloning support. Non-commercial research license. |
| DeepMine-multi-TTS | https://dl.acm.org/doi/abs/10.1007/s10579-025-09807-6 | 120 hours of high-quality Persian speech from 67 speakers for multi-speaker TTS. |
| Matina (Persian Text Corpus) | https://huggingface.co/datasets/MLChina/Matina | Large-scale 73B token Persian text corpus for LLM pre-training. |
| PersianMedQA | https://huggingface.co/datasets/MohammadJRanjbar/PersianMedQA | Over 20,000 expert-validated medical questions from Iranian national board exams for evaluating Persian medical AI. |
| PersianSciQA | https://huggingface.co/datasets/PersianSciQA/PersianSciQA | Dataset for bridging the language gap in scientific question answering in Persian. |
| Common Voice (Persian) | https://huggingface.co/datasets/mozilla-foundation/common_voice_13_0 | Mozilla Common Voice Persian subset for ASR training. |
| artindnr/poem-generation-1k | https://huggingface.co/datasets/artindnr/poem-generation-1k | 1,000 Persian poem entries for poetry generation fine-tuning. |
| mauxi-mix-persian | https://huggingface.co/datasets/xmanii/mauxi-mix-persian | Mixed Persian dataset for multi-task training. |

---

## Benchmarks & Leaderboards

| Benchmark | Link | Description |
|-----------|------|-------------|
| Open Persian LLM Leaderboard | https://huggingface.co/spaces/PartAI/open-persian-llm-leaderboard | Leaderboard by Part AI and AUT NLP Lab for evaluating Persian LLMs on six specialized tasks with 40,000+ samples. Submit your model for evaluation. |
| ParsBench | https://github.com/ParsBench/parsbench | Benchmarking toolset for Persian LLMs covering sentiment analysis, machine translation, MCQ, using ParsiNLU and Persian-MMLU datasets. |
| MofidAI Persian NLP Benchmark | https://github.com/mofidAI/persian-nlp-benchmark | Benchmarks HuggingFace Persian models (mT5, BERT) across 12,712 available datasets. |
| ParsiNLU | https://huggingface.co/datasets/ParsiNLU | Benchmark suite for Persian natural language understanding tasks. |
| Persian-MMLU | https://huggingface.co/datasets/Persian-MMLU | Persian version of MMLU for evaluating LLM knowledge in Farsi. |

---

## Tools & Frameworks

| Tool | Link | Description |
|------|------|-------------|
| Hezar | https://github.com/hezarai/hezar | Open-source multipurpose AI toolkit for Persian. Unified Python interface for loading, training, and using models for text generation, sentiment analysis, ASR, and OCR. |
| Persian-TTS-Zoo | https://github.com/Adibian/Persian-TTS-Zoo | Curated collection of open-source Persian TTS projects including Tacotron2, FastSpeech2, GST-Tacotron, and HiFiGAN implementations. |
| PersianML (Community) | https://huggingface.co/PersianML | Persian AI community developing open models, datasets, and benchmarks for Persian text, speech, OCR, and multimodal AI. |
| ZabanZad.ai | https://sail-lab.org/portfolio/persian-nlp-advancement-for-enhanced-farsi-language-ai | Open-source initiative for Persian TTS datasets and models, led by SAIL Lab. |
| Persian-tts-coqui | https://github.com/karim23657/Persian-tts-coqui | Persian TTS models, demos, and training code using the Coqui TTS framework. |

---

## License

This repository itself is licensed under the MIT License — see the [LICENSE](LICENSE) file for details. Each linked model or dataset has its own license; please check the original source before use.
