# Research-Recommendation
This repository leverages HuggingFace libraries and artifacts, including Transformers, GPT-2, and transformer reinforcement learning (TRL) to fine-tune GPT-2 on a curated data set of user-topic pairs to enable predictions about topics that a new user would like. For each topic prediction, relevant research articles are returned.

# Research paper

The PDF explaining this research in-depth is included in this repository.

# Notebooks
The dataset engineering notebook contains processes to convert from the CiteULike dataset (an old web app that allowed users to tag which topics they liked) to a useable dataset for finetuning GPT-2 with HuggingFace.

The Finetuning notebook leverages the above dataset to finetune GPT-2.

The "FT^2" notebook leverages proximal policy optimization to finetune GPT-2 based on active user feedback (from the Gradio UI) on their preferences for recommended topics.
