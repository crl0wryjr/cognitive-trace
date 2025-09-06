# Cognitive Trace

## Overview

Cognitive Trace is a framework for exposing the reasoning patterns, strategies, and execution steps that Large Language Models (LLMs) use when responding to prompts. By providing visibility into what is typically a black-box process, this tool enables users to inspect the 'how and why' behind LLM responses, making it an invaluable resource for prompt debugging and optimization.

There are two main components to this framework:  Scratchpads and Metacognitive Prompting.

## What are Scratchpads?

Scratchpads are a type of working memory available to LLMs, most often used in __Chain of ..._ style prompts. With many LLMs this feature is turned off by deafult, and even when enabled, the contents of the scratchpad is not usually shared with the user.

With this framework I am exposing the LLM's scratchpad,  giving us insight into the reasoning processes thats occur during response generation. Think of this as a debugging tool for AI-generated output.

## Key Features

- **Reasoning Transparency**: Visual inspection of LLM decision-making processes
- **Prompt Optimization**: Tools for troubleshooting and improving user prompts
- **Strategy Analysis**: Understanding of different reasoning strategies employed by LLMs
- **Execution Step Tracking**: Detailed view of how LLMs approach complex problems

## What is Metacognitive Prompting

Metacognitive Prompting is a framework intended to mimic the way a human being reasons. In the paper [Metacognitive Prompting Improves Understanding in Large Language Models](https://arxiv.org/abs/2308.05342) Yuqing Wang describes MP as:
> Derived from cognitive psychology, metacognition relates to an individual’s awareness and self-reflection on their cognitive processes. Our ap-proach integrates key aspects of human metacognitive processes into LLMs.

## Research Background

This work is inspired by extensive research on both Metacongnitive Prompting and scratchpads, and their role in improving __Chain of ...__ style reasoning in language models. 

My initial idea for utilizing scratchpads to expose LLM reasoning and output comes from four, somewhat terrifying studies exploring how LLMs will knowlingly act in deceptive ways:

* [SLEEPER AGENTS: TRAINING DECEPTIVE LLMS THAT PERSIST THROUGH SAFETY TRAINING](https://arxiv.org/abs/2401.05566)
* [Language Models Don’t Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompts](https://arxiv.org/abs/2305.04388)
* [Measuring Faithfulness in Chain-of-Thought Reasoning](https://arxiv.org/abs/2307.13702)
* [ALIGNMENT FAKING IN LARGE LANGUAGE MODELS](https://assets.anthropic.com/m/983c85a201a962f/original/Alignment-Faking-in-Large-Language-Models-full-paper.pdf)


My introduction to Metacognitive Prompting / Thought Calibration come from these three sources:
* [Thought calibration: Efficient and confident test-time scaling](https://arxiv.org/abs/2308.05342)
* [Metacognitive Prompting Improves Understanding in Large Language Models](https://arxiv.org/abs/2308.05342)
* [Para-Droid-AI's Scratchpad project on GitHub](https://github.com/para-droid-ai/scratchpad/blob/main/README.md)


## Usage

*Usage examples and documentation will be added here*

## Future Direction

* Invesitage the effectiveness of a Scratchpad / Metacongitive prompt as the default basis for custom instructions
* Creating an On / Off switch for scratchpad visibility
* Dynamically pulling in / exlcuing aspects of the MP framework


## Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

## License

*License information will be added here*
