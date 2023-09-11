[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

## Updated on 2023.09.11

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href=#diffusion>diffusion</a></li>
  </ol>
</details>

## diffusion

|Date|Title|label|Abstract|PDF|Code|
|---|---|---|---|---|---|
|**2023-09-02**|**Bridge Diffusion Model: bridge non-English language-native text-to-image diffusion model with English communities**|cs.CL, cs.AI|Text-to-Image generation (TTI) technologies are advancing rapidly, especially in the English language communities. However, English-native TTI models inherently carry biases from English world centric training data, which creates a dilemma for development of other language-native TTI models. One common choice is fine-tuning the English-native TTI model with translated samples from non-English communities. It falls short of fully addressing the model bias problem. Alternatively, training non-English language native models from scratch can effectively resolve the English world bias, but diverges from the English TTI communities, thus not able to utilize the strides continuously gaining in the English TTI communities any more. To build non-English language native TTI model meanwhile keep compatability with the English TTI communities, we propose a novel model structure referred as "Bridge Diffusion Model" (BDM). The proposed BDM employs a backbone-branch network structure to learn the non-English language semantics while keep the latent space compatible with the English-native TTI backbone, in an end-to-end manner. The unique advantages of the proposed BDM are that it's not only adept at generating images that precisely depict non-English language semantics, but also compatible with various English-native TTI plugins, such as different checkpoints, LoRA, ControlNet, Dreambooth, and Textual Inversion, etc. Moreover, BDM can concurrently generate content seamlessly combining both non-English native and English-native semantics within a single image, fostering cultural interaction. We verify our method by applying BDM to build a Chinese-native TTI model, whereas the method is generic and applicable to any other language. |[2309.00952v1](http://arxiv.org/abs/2309.00952v1)|null|
|**2023-09-04**|**ParaGuide: Guided Diffusion Paraphrasers for Plug-and-Play Textual Style Transfer**|cs.CL, cs.AI|Textual style transfer is the task of transforming stylistic properties of text while preserving meaning. Target "styles" can be defined in numerous ways, ranging from single attributes (e.g, formality) to authorship (e.g, Shakespeare). Previous unsupervised style-transfer approaches generally rely on significant amounts of labeled data for only a fixed set of styles or require large language models. In contrast, we introduce a novel diffusion-based framework for general-purpose style transfer that can be flexibly adapted to arbitrary target styles at inference time. Our parameter-efficient approach, ParaGuide, leverages paraphrase-conditioned diffusion models alongside gradient-based guidance from both off-the-shelf classifiers and strong existing style embedders to transform the style of text while preserving semantic information. We validate the method on the Enron Email Corpus, with both human and automatic evaluations, and find that it outperforms strong baselines on formality, sentiment, and even authorship style transfer. |[2308.15459v2](http://arxiv.org/abs/2308.15459v2)|**[link](https://github.com/zacharyhorvitz/ParaGuide)**|
|**2023-08-25**|**Diffusion Language Models Can Perform Many Tasks with Scaling and Instruction-Finetuning**|cs.CL, cs.AI, cs.LG|The recent surge of generative AI has been fueled by the generative power of diffusion probabilistic models and the scalable capabilities of large language models. Despite their potential, it remains elusive whether diffusion language models can solve general language tasks comparable to their autoregressive counterparts. This paper demonstrates that scaling diffusion models w.r.t. data, sizes, and tasks can effectively make them strong language learners. We build competent diffusion language models at scale by first acquiring knowledge from massive data via masked language modeling pretraining thanks to their intrinsic connections. We then reprogram pretrained masked language models into diffusion language models via diffusive adaptation, wherein task-specific finetuning and instruction finetuning are explored to unlock their versatility in solving general language tasks. Experiments show that scaling diffusion language models consistently improves performance across downstream language tasks. We further discover that instruction finetuning can elicit zero-shot and few-shot in-context learning abilities that help tackle many unseen tasks by following natural language instructions, and show promise in advanced and challenging abilities such as reasoning. |[2308.12219v2](http://arxiv.org/abs/2308.12219v2)|**[link](https://github.com/yegcjs/diffusionllm)**|
|**2023-08-23**|**Audio Generation with Multiple Conditional Diffusion Model**|cs.SD, cs.CL, cs.LG, eess.AS|Text-based audio generation models have limitations as they cannot encompass all the information in audio, leading to restricted controllability when relying solely on text. To address this issue, we propose a novel model that enhances the controllability of existing pre-trained text-to-audio models by incorporating additional conditions including content (timestamp) and style (pitch contour and energy contour) as supplements to the text. This approach achieves fine-grained control over the temporal order, pitch, and energy of generated audio. To preserve the diversity of generation, we employ a trainable control condition encoder that is enhanced by a large language model and a trainable Fusion-Net to encode and fuse the additional conditions while keeping the weights of the pre-trained text-to-audio model frozen. Due to the lack of suitable datasets and evaluation metrics, we consolidate existing datasets into a new dataset comprising the audio and corresponding conditions and use a series of evaluation metrics to evaluate the controllability performance. Experimental results demonstrate that our model successfully achieves fine-grained control to accomplish controllable audio generation. Audio samples and our dataset are publicly available at https://conditionaudiogen.github.io/conditionaudiogen/ |[2308.11940v1](http://arxiv.org/abs/2308.11940v1)|null|
|**2023-08-17**|**Enhancing Phrase Representation by Information Bottleneck Guided Text Diffusion Process for Keyphrase Extraction**|cs.CL|Keyphrase extraction (KPE) is an important task in Natural Language Processing for many scenarios, which aims to extract keyphrases that are present in a given document. Many existing supervised methods treat KPE as sequential labeling, span-level classification, or generative tasks. However, these methods lack the ability to utilize keyphrase information, which may result in biased results. In this study, we propose Diff-KPE, which leverages the supervised Variational Information Bottleneck (VIB) to guide the text diffusion process for generating enhanced keyphrase representations. Diff-KPE first generates the desired keyphrase embeddings conditioned on the entire document and then injects the generated keyphrase embeddings into each phrase representation. A ranking network and VIB are then optimized together with rank loss and classification loss, respectively. This design of Diff-KPE allows us to rank each candidate phrase by utilizing both the information of keyphrases and the document. Experiments show that Diff-KPE outperforms existing KPE methods on a large open domain keyphrase extraction benchmark, OpenKP, and a scientific domain dataset, KP20K. |[2308.08739v1](http://arxiv.org/abs/2308.08739v1)|null|
|**2023-07-31**|**Comparing normalizing flows and diffusion models for prosody and acoustic modelling in text-to-speech**|eess.AS, cs.CL, cs.LG|Neural text-to-speech systems are often optimized on L1/L2 losses, which make strong assumptions about the distributions of the target data space. Aiming to improve those assumptions, Normalizing Flows and Diffusion Probabilistic Models were recently proposed as alternatives. In this paper, we compare traditional L1/L2-based approaches to diffusion and flow-based approaches for the tasks of prosody and mel-spectrogram prediction for text-to-speech synthesis. We use a prosody model to generate log-f0 and duration features, which are used to condition an acoustic model that generates mel-spectrograms. Experimental results demonstrate that the flow-based model achieves the best performance for spectrogram prediction, improving over equivalent diffusion and L1 models. Meanwhile, both diffusion and flow-based prosody predictors result in significant improvements over a typical L2-trained prosody models. |[2307.16679v1](http://arxiv.org/abs/2307.16679v1)|null|
|**2023-07-31**|**DiffProsody: Diffusion-based Latent Prosody Generation for Expressive Speech Synthesis with Prosody Conditional Adversarial Training**|cs.SD, cs.CL, eess.AS|Expressive text-to-speech systems have undergone significant advancements owing to prosody modeling, but conventional methods can still be improved. Traditional approaches have relied on the autoregressive method to predict the quantized prosody vector; however, it suffers from the issues of long-term dependency and slow inference. This study proposes a novel approach called DiffProsody in which expressive speech is synthesized using a diffusion-based latent prosody generator and prosody conditional adversarial training. Our findings confirm the effectiveness of our prosody generator in generating a prosody vector. Furthermore, our prosody conditional discriminator significantly improves the quality of the generated speech by accurately emulating prosody. We use denoising diffusion generative adversarial networks to improve the prosody generation speed. Consequently, DiffProsody is capable of generating prosody 16 times faster than the conventional diffusion model. The superior performance of our proposed method has been demonstrated via experiments. |[2307.16549v1](http://arxiv.org/abs/2307.16549v1)|**[link](https://github.com/hsoh0306/diffprosody)**|
|**2023-07-28**|**Minimally-Supervised Speech Synthesis with Conditional Diffusion Model and Language Model: A Comparative Study of Semantic Coding**|cs.SD, cs.AI, cs.CL, eess.AS|Recently, there has been a growing interest in text-to-speech (TTS) methods that can be trained with minimal supervision by combining two types of discrete speech representations and using two sequence-to-sequence tasks to decouple TTS. To address the challenges associated with high dimensionality and waveform distortion in discrete representations, we propose Diff-LM-Speech, which models semantic embeddings into mel-spectrogram based on diffusion models and introduces a prompt encoder structure based on variational autoencoders and prosody bottlenecks to improve prompt representation capabilities. Autoregressive language models often suffer from missing and repeated words, while non-autoregressive frameworks face expression averaging problems due to duration prediction models. To address these issues, we propose Tetra-Diff-Speech, which designs a duration diffusion model to achieve diverse prosodic expressions. While we expect the information content of semantic coding to be between that of text and acoustic coding, existing models extract semantic coding with a lot of redundant information and dimensionality explosion. To verify that semantic coding is not necessary, we propose Tri-Diff-Speech. Experimental results show that our proposed methods outperform baseline methods. We provide a website with audio samples. |[2307.15484v1](http://arxiv.org/abs/2307.15484v1)|null|
|**2023-07-26**|**Diff-E: Diffusion-based Learning for Decoding Imagined Speech EEG**|eess.AS, cs.CL, cs.HC, cs.LG, 68T10|Decoding EEG signals for imagined speech is a challenging task due to the high-dimensional nature of the data and low signal-to-noise ratio. In recent years, denoising diffusion probabilistic models (DDPMs) have emerged as promising approaches for representation learning in various domains. Our study proposes a novel method for decoding EEG signals for imagined speech using DDPMs and a conditional autoencoder named Diff-E. Results indicate that Diff-E significantly improves the accuracy of decoding EEG signals for imagined speech compared to traditional machine learning techniques and baseline models. Our findings suggest that DDPMs can be an effective tool for EEG signal decoding, with potential implications for the development of brain-computer interfaces that enable communication through imagined speech. |[2307.14389v1](http://arxiv.org/abs/2307.14389v1)|**[link](https://github.com/yorgoon/diffe)**|
|**2023-07-26**|**Founding a mathematical diffusion model in linguistics. The case study of German syntactic features in the North-Eastern Italian dialects**|cs.CL|We take as a case study the spread of Germanic syntactic features into Romance dialects of North-Eastern Italy, which occurred after the immigration of German people in the Tyrol during the High Middle Ages.   An interactive map is produced using tools of what is called Geographic Data Science. A smooth two-dimensional surface $\mathcal{G}$ expresses locally which fraction of territory uses a given German language feature: it is obtained by interpolating a discrete function that says if at any surveyed locality that feature is used or not.\newline   This surface $\mathcal{G}$ is thought of as the value at the present time of a function describing a diffusion-convection phenomenon in two dimensions (here said \emph{tidal} mode), which is subjected in a very natural way to the same equation, suitably contextualized, used in physics for a number of phenomenological facts like the heat diffusion. It is shown that solutions of this equation, evaluated at the present time, fit well with the data as interpolated by $\mathcal{G}$, thus providing convincing pictures of diffusion-convection of the linguistic features of the case study, albeit simplifications and approximations.\newline   Very importantly, it is shown that Schmidt's 'waves' can be counted among the solutions of the diffusion equation: superimposing Schmidt 'waves' to a 'tidal flooding' can reproduce complexities of real linguistic diffusion events. |[2307.14291v1](http://arxiv.org/abs/2307.14291v1)|null|
|**2023-07-26**|**How Does Diffusion Influence Pretrained Language Models on Out-of-Distribution Data?**|cs.CL, cs.AI|Transformer-based pretrained language models (PLMs) have achieved great success in modern NLP. An important advantage of PLMs is good out-of-distribution (OOD) robustness. Recently, diffusion models have attracted a lot of work to apply diffusion to PLMs. It remains under-explored how diffusion influences PLMs on OOD data. The core of diffusion models is a forward diffusion process which gradually applies Gaussian noise to inputs, and a reverse denoising process which removes noise. The noised input reconstruction is a fundamental ability of diffusion models. We directly analyze OOD robustness by measuring the reconstruction loss, including testing the abilities to reconstruct OOD data, and to detect OOD samples. Experiments are conducted by analyzing different training parameters and data statistical features on eight datasets. It shows that finetuning PLMs with diffusion degrades the reconstruction ability on OOD data. The comparison also shows that diffusion models can effectively detect OOD samples, achieving state-of-the-art performance in most of the datasets with an absolute accuracy improvement up to 18%. These results indicate that diffusion reduces OOD robustness of PLMs. |[2307.13949v1](http://arxiv.org/abs/2307.13949v1)|**[link](https://github.com/maybelizzy/diffusion_ood_robustness)**|
|**2023-07-31**|**XDLM: Cross-lingual Diffusion Language Model for Machine Translation**|cs.CL|Recently, diffusion models have excelled in image generation tasks and have also been applied to neural language processing (NLP) for controllable text generation. However, the application of diffusion models in a cross-lingual setting is less unexplored. Additionally, while pretraining with diffusion models has been studied within a single language, the potential of cross-lingual pretraining remains understudied. To address these gaps, we propose XDLM, a novel Cross-lingual diffusion model for machine translation, consisting of pretraining and fine-tuning stages. In the pretraining stage, we propose TLDM, a new training objective for mastering the mapping between different languages; in the fine-tuning stage, we build up the translation system based on the pretrained model. We evaluate the result on several machine translation benchmarks and outperformed both diffusion and Transformer baselines. |[2307.13560v2](http://arxiv.org/abs/2307.13560v2)|null|
|**2023-07-09**|**Augmenters at SemEval-2023 Task 1: Enhancing CLIP in Handling Compositionality and Ambiguity for Zero-Shot Visual WSD through Prompt Augmentation and Text-To-Image Diffusion**|cs.CL|This paper describes our zero-shot approaches for the Visual Word Sense Disambiguation (VWSD) Task in English. Our preliminary study shows that the simple approach of matching candidate images with the phrase using CLIP suffers from the many-to-many nature of image-text pairs. We find that the CLIP text encoder may have limited abilities in capturing the compositionality in natural language. Conversely, the descriptive focus of the phrase varies from instance to instance. We address these issues in our two systems, Augment-CLIP and Stable Diffusion Sampling (SD Sampling). Augment-CLIP augments the text prompt by generating sentences that contain the context phrase with the help of large language models (LLMs). We further explore CLIP models in other languages, as the an ambiguous word may be translated into an unambiguous one in the other language. SD Sampling uses text-to-image Stable Diffusion to generate multiple images from the given phrase, increasing the likelihood that a subset of images match the one that paired with the text. |[2307.05564v1](http://arxiv.org/abs/2307.05564v1)|null|
|**2023-06-14**|**DiffuDetox: A Mixed Diffusion Model for Text Detoxification**|cs.CL, cs.LG|Text detoxification is a conditional text generation task aiming to remove offensive content from toxic text. It is highly useful for online forums and social media, where offensive content is frequently encountered. Intuitively, there are diverse ways to detoxify sentences while preserving their meanings, and we can select from detoxified sentences before displaying text to users. Conditional diffusion models are particularly suitable for this task given their demonstrated higher generative diversity than existing conditional text generation models based on language models. Nonetheless, text fluency declines when they are trained with insufficient data, which is the case for this task. In this work, we propose DiffuDetox, a mixed conditional and unconditional diffusion model for text detoxification. The conditional model takes toxic text as the condition and reduces its toxicity, yielding a diverse set of detoxified sentences. The unconditional model is trained to recover the input text, which allows the introduction of additional fluent text for training and thus ensures text fluency. Extensive experimental results and in-depth analysis demonstrate the effectiveness of our proposed DiffuDetox. |[2306.08505v1](http://arxiv.org/abs/2306.08505v1)|null|
|**2023-06-13**|**StyleTTS 2: Towards Human-Level Text-to-Speech through Style Diffusion and Adversarial Training with Large Speech Language Models**|eess.AS, cs.AI, cs.CL, cs.LG, cs.SD|In this paper, we present StyleTTS 2, a text-to-speech (TTS) model that leverages style diffusion and adversarial training with large speech language models (SLMs) to achieve human-level TTS synthesis. StyleTTS 2 differs from its predecessor by modeling styles as a latent random variable through diffusion models to generate the most suitable style for the text without requiring reference speech, achieving efficient latent diffusion while benefiting from the diverse speech synthesis offered by diffusion models. Furthermore, we employ large pre-trained SLMs, such as WavLM, as discriminators with our novel differentiable duration modeling for end-to-end training, resulting in improved speech naturalness. StyleTTS 2 surpasses human recordings on the single-speaker LJSpeech dataset and matches it on the multispeaker VCTK dataset as judged by native English speakers. Moreover, when trained on the LibriTTS dataset, our model outperforms previous publicly available models for zero-shot speaker adaptation. This work achieves the first human-level TTS on both single and multispeaker datasets, showcasing the potential of style diffusion and adversarial training with large SLMs. The audio demos and source code are available at https://styletts2.github.io/. |[2306.07691v1](http://arxiv.org/abs/2306.07691v1)|null|
|**2023-06-05**|**PLANNER: Generating Diversified Paragraph via Latent Language Diffusion Model**|cs.CL|Autoregressive models for text sometimes generate repetitive and low-quality output because errors accumulate during the steps of generation. This issue is often attributed to exposure bias - the difference between how a model is trained, and how it is used during inference. Denoising diffusion models provide an alternative approach in which a model can revisit and revise its output. However, they can be computationally expensive and prior efforts on text have led to models that produce less fluent output compared to autoregressive models, especially for longer text and paragraphs. In this paper, we propose PLANNER, a model that combines latent semantic diffusion with autoregressive generation, to generate fluent text while exercising global control over paragraphs. The model achieves this by combining an autoregressive "decoding" module with a "planning" module that uses latent diffusion to generate semantic paragraph embeddings in a coarse-to-fine manner. The proposed method is evaluated on various conditional generation tasks, and results on semantic generation, text completion and summarization show its effectiveness in generating high-quality long-form text in an efficient manner. |[2306.02531v1](http://arxiv.org/abs/2306.02531v1)|null|
|**2023-06-02**|**DiffusEmp: A Diffusion Model-Based Framework with Multi-Grained Control for Empathetic Response Generation**|cs.CL, cs.AI|Empathy is a crucial factor in open-domain conversations, which naturally shows one's caring and understanding to others. Though several methods have been proposed to generate empathetic responses, existing works often lead to monotonous empathy that refers to generic and safe expressions. In this paper, we propose to use explicit control to guide the empathy expression and design a framework DiffusEmp based on conditional diffusion language model to unify the utilization of dialogue context and attribute-oriented control signals. Specifically, communication mechanism, intent, and semantic frame are imported as multi-grained signals that control the empathy realization from coarse to fine levels. We then design a specific masking strategy to reflect the relationship between multi-grained signals and response tokens, and integrate it into the diffusion model to influence the generative process. Experimental results on a benchmark dataset EmpatheticDialogue show that our framework outperforms competitive baselines in terms of controllability, informativeness, and diversity without the loss of context-relatedness. |[2306.01657v1](http://arxiv.org/abs/2306.01657v1)|null|
|**2023-05-31**|**Fine-grained Text Style Transfer with Diffusion-Based Language Models**|cs.CL, cs.AI, cs.LG|Diffusion probabilistic models have shown great success in generating high-quality images controllably, and researchers have tried to utilize this controllability into text generation domain. Previous works on diffusion-based language models have shown that they can be trained without external knowledge (such as pre-trained weights) and still achieve stable performance and controllability. In this paper, we trained a diffusion-based model on StylePTB dataset, the standard benchmark for fine-grained text style transfers. The tasks in StylePTB requires much more refined control over the output text compared to tasks evaluated in previous works, and our model was able to achieve state-of-the-art performance on StylePTB on both individual and compositional transfers. Moreover, our model, trained on limited data from StylePTB without external knowledge, outperforms previous works that utilized pretrained weights, embeddings, and external grammar parsers, and this may indicate that diffusion-based language models have great potential under low-resource settings. |[2305.19512v1](http://arxiv.org/abs/2305.19512v1)|**[link](https://github.com/lvyiwei1/diffuseq_styleptb)**|
|**2023-05-30**|**Likelihood-Based Diffusion Language Models**|cs.CL, cs.LG|Despite a growing interest in diffusion-based language models, existing work has not shown that these models can attain nontrivial likelihoods on standard language modeling benchmarks. In this work, we take the first steps towards closing the likelihood gap between autoregressive and diffusion-based language models, with the goal of building and releasing a diffusion model which outperforms a small but widely-known autoregressive model. We pursue this goal through algorithmic improvements, scaling laws, and increased compute. On the algorithmic front, we introduce several methodological improvements for the maximum-likelihood training of diffusion language models. We then study scaling laws for our diffusion models and find compute-optimal training regimes which differ substantially from autoregressive models. Using our methods and scaling analysis, we train and release Plaid 1B, a large diffusion language model which outperforms GPT-2 124M in likelihood on benchmark datasets and generates fluent samples in unconditional and zero-shot control settings. |[2305.18619v1](http://arxiv.org/abs/2305.18619v1)|**[link](https://github.com/igul222/plaid)**|

<p align=right>(<a href=#Updated-on-20230911>back to top</a>)</p>

[contributors-shield]: https://img.shields.io/github/contributors/bansky-cl/diffusion-nlp-paper-arxiv.svg?style=for-the-badge
[contributors-url]: https://github.com/bansky-cl/diffusion-nlp-paper-arxiv/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/bansky-cl/diffusion-nlp-paper-arxiv.svg?style=for-the-badge
[forks-url]: https://github.com/bansky-cl/diffusion-nlp-paper-arxiv/network/members
[stars-shield]: https://img.shields.io/github/stars/bansky-cl/diffusion-nlp-paper-arxiv.svg?style=for-the-badge
[stars-url]: https://github.com/bansky-cl/diffusion-nlp-paper-arxiv/stargazers
[issues-shield]: https://img.shields.io/github/issues/bansky-cl/diffusion-nlp-paper-arxiv.svg?style=for-the-badge
[issues-url]: https://github.com/bansky-cl/diffusion-nlp-paper-arxiv/issues

