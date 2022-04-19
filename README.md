## library used:

### 1. Librosa:
librosa is a python package for music and audio analysis. It provides the building blocks necessary to create music information retrieval systems.
https://librosa.org/doc/latest/index.html

### 2. Torch:

Torch comes with a large ecosystem of community-driven packages in machine learning, computer vision, signal processing, parallel processing, image, video, audio and networking among others, and builds on top of the Lua community. http://torch.ch/

### 3. IPython:
IPython provides a rich toolkit to help you make the most of using Python interactively.
https://ipython.readthedocs.io/en/stable/

### 4. Transformers:
Transformers provides thousands of pretrained models to perform tasks on different modalities such as text, vision, and audio. https://github.com/huggingface/transformers

These models can be applied on:

📝 Text, for tasks like text classification, information extraction, question answering, summarization, translation, text generation, in over 100 languages.

🖼️ Images, for tasks like image classification, object detection, and segmentation.

🗣️ Audio, for tasks like speech recognition and audio classification.


## Task 1 Explanation:

Play audio to check rate:
Facebook library(**"facebook/wav2vec2-base-960h"**) requires audio file sampling rate=16000Hz to run through pipeline.

Wav2Vec2- https://huggingface.co/docs/transformers/model_doc/wav2vec2 . 
This pretrained facebook model is used for audio to text classification

Data is an array essentially consist of various parametes like frame rate, sampling rate,duration of audio file.
In the given **sales_call_telephone_marketers.wav** audio file which has **sample rate:  16000 Hz** & **Total time:  48.691375 s**. 

Then tokenize input values passed it through model take maximum prediction from logit and then extract the text

## Task 4 Explanation:

Summarization: 
Summarization is the task of producing a shorter version of a document while preserving its important information.
Some models can extract text from the original input, while other models can generate entirely new text.
https://huggingface.co/tasks/summarization

 If no model name is provided the pipeline will be initialized with **sshleifer/distilbart-cnn-12-6** .
