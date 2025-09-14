# Cognitive Trace

## Overview

Cognitive Trace is a framework for exposing the reasoning patterns, strategies, and execution steps that Large Language Models (LLMs) use when responding to prompts. By providing visibility into what is typically a black-box process, this framework enables users to inspect the 'how and why' behind LLM responses, making it an invaluable resource for prompt debugging and optimization.


## Usage

#### Cognitive Trace - v1.0 & Cognitive Trace - Proof of Concept
1. Paste the contents of "Prompt - CognitiveTrace.md" into a GPT conversation (do **NOT** submit)
2. Add the remainder of your prompt, followed with [S],[M], or [L]
4. Read through the cognitive trace, making corrections and updates as needed
5. Tell the system to "Proceed"

#### Example 
``` TEXT
USER PASTED:  {Prompt - CognitiveTrace.md}

USER TYPED:  Explain how AI based SEO will change traditional SEO [L] <ENTER>

SYSTEM RESPONSE:  {cognitive trace output}

USER TYPED:  Proceed <ENTER>
```


## There are two main components to this framework:  Scratchpads and Metacognitive Prompting.

### What are Scratchpads?

Scratchpads are a type of working memory available to LLMs, most often used in _Chain of ..._ style prompts. With many LLMs this feature is turned off by deafult, and even when enabled, the contents of the scratchpad is not usually shared with the user.

With this framework I am exposing the LLM's scratchpad,  giving us insight into the reasoning processes thats occur during response generation. Think of this as a debugging tool for AI-generated output.

### Key Features

- **Reasoning Transparency**: Visual inspection of LLM decision-making processes
- **Strategy Analysis**: Understanding of different reasoning strategies employed by LLMs
- **Execution Step Tracking**: Detailed view of how LLMs approach complex problems

### What is Metacognitive Prompting

Metacognitive Prompting is a framework intended to mimic the way a human being reasons. 
In the paper [Metacognitive Prompting Improves Understanding in Large Language Models](https://arxiv.org/abs/2308.05342) Yuqing Wang describes MP as:
> Derived from cognitive psychology, metacognition relates to an individual’s awareness and self-reflection on their cognitive processes. Our approach integrates key aspects of human metacognitive processes into LLMs.

### Key Features

- **Improved Reliability**: Metacognition techniques have shown improvements in the accuracy of  _Chain of ..._ style prompts
- **Improved Readability**: Well defined sections & guidelines


## Research Background

This work is inspired by extensive research on both Metacongnitive Prompting and scratchpads, and their role in improving _Chain of ..._ style reasoning in LLMs. 

The initial idea for utilizing scratchpads to expose LLM reasoning and output comes from four, somewhat terrifying studies exploring how LLMs will knowlingly act in deceptive ways:

* [SLEEPER AGENTS: TRAINING DECEPTIVE LLMS THAT PERSIST THROUGH SAFETY TRAINING](https://arxiv.org/abs/2401.05566)
* [Language Models Don’t Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompts](https://arxiv.org/abs/2305.04388)
* [Measuring Faithfulness in Chain-of-Thought Reasoning](https://arxiv.org/abs/2307.13702)
* [ALIGNMENT FAKING IN LARGE LANGUAGE MODELS](https://assets.anthropic.com/m/983c85a201a962f/original/Alignment-Faking-in-Large-Language-Models-full-paper.pdf)


My introduction to Metacognitive Prompting / Thought Calibration primarily comes from these three sources:

* [Thought calibration: Efficient and confident test-time scaling](https://arxiv.org/abs/2308.05342)
* [Metacognitive Prompting Improves Understanding in Large Language Models](https://arxiv.org/abs/2308.05342)
* [Para-Droid-AI's Scratchpad project on GitHub](https://github.com/para-droid-ai/scratchpad/blob/main/README.md)

These sources, as well as several others, position Metacognitive Prompting & Thought Calibration as a means of dramatically improving an LLM's execution of complext tasks, by mimicing a human reasoning process;  as opposed to the linear, next-token based reasoning that is default. I have not performed any testing of my own, relying instead on the well documented and peer reviewed research of those far more knowledgeable than me. My initial goal has been the use of MP / TC as a formatting structure allowing for easy scanability of the exposed scratchpad. As I evolve the framework I will likely investigate real world performance & reliability.


## Future Direction

* Linguistic copression and prompt optimizations
* Invesitage the effectiveness of a Scratchpad / Metacongitive prompt as the default basis for custom instructions
* Creating an On / Off switch for scratchpad visibility
* Dynamically including / excluding aspects of the MP framework


## Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.


## License

### MIT License
**Copyright (c) 2025, Rob Lowry**

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
