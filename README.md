# Research-Recommendation
This repository leverages HuggingFace libraries and artifacts, including Transformers, GPT-2, and transformer reinforcement learning (TRL) to fine-tune GPT-2 on a curated data set of user-topic pairs to enable predictions about topics that a new user would like. For each topic prediction, relevant research articles are returned based on search queries run against the open source "OpenAlex" database of academic research.

The goals of this project are threefold:

(1) Create a product which takes, as input, topics that a researcher is already interested in and
returns a novel topic-of-interest each time it is called.

(2) Return a handful of research documents related to that topic along with some useful metainformation about those documents.

(3) Equip the system to learn, over a series of time steps, to recommend increasingly better
topics according to the user’s inputs and feedback.


# Research paper

The PDF explaining this research in-depth is included in this repository.

# Notebooks
The dataset engineering notebook contains processes to convert from the CiteULike dataset (an old web app that allowed users to tag which topics they liked) to a useable dataset for finetuning GPT-2 with HuggingFace.

The Finetuning notebook leverages the above dataset to finetune GPT-2.

The "FT^2" notebook leverages proximal policy optimization to finetune GPT-2 based on active user feedback (from the Gradio UI) on their preferences for recommended topics.
