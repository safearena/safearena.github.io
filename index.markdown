---
layout: default
---

<div align="center">

<h1>SafeArena</h1>
<h2>Evaluating Safety in Autonomous Web Agents</h2>

Ada Tur<sup>*</sup> &nbsp; Nicholas Meade<sup>*</sup> &nbsp; Xing Han Lù<sup>*</sup> &nbsp; Alejandra Zambrano<sup>†</sup> &nbsp; Arkil Patel<sup>†</sup>
<br>
&nbsp; Esin Durmus &nbsp; Spandana Gella &nbsp; Karolina Stańczak &nbsp; Siva Reddy
<br>
<br>
<sup>*</sup>Equal Contribution

<table>
      <tr>
            <td>
                  <a href="https://github.com/McGill-NLP/safearena">💻 GitHub</a>
            </td>
            <td>
                  <a href="404.html">📄 Paper</a>
            </td>
            <td>
                  <a href="404.html">📊 Leaderboard</a>
            </td>
      </tr>
</table>

</div>

## Are Web Agents Safe?

LLM-based agents are becoming increasingly proficient at solving web-based tasks. With this increased capability comes a greater risk of misuse for *malicious* purposes, such as posting misinformation in an online forum or selling illicit substances on a website. To evaluate these risks, we propose **SafeArena**, the first benchmark to focus on the deliberate misuse of web agents.

<img src="/assets/safearena_fig1_v2.jpg" alt="SafeArena Fig1">

## SafeArena

**SafeArena** comprises 250 safe and 250 harmful tasks across four websites. We classify the harmful tasks into five harm categories---*misinformation*, *illegal activity*, *harassment*, *cybercrime*, and *social bias*---designed to assess realistic misuses of web agents.

## How Do Current Agents Perform?

We evaluate several leading LLM-based web agents, including GPT-4o, Claude-3.5 Sonnet, Qwen-2 72B, and Llama-3.2 90B, on our benchmark. 

Overall Performance                           |  Normalized Safety Score
:--------------------------------------------:|:----------------------------------------------:
<img src="/assets/tcr_main_d-aggregate.jpg" width=500px>  |  <img src="/assets/tcr_main_d-normalized_safety.jpg" width=500px>

We find that agents are surprisingly compliant with malicious requests, with GPT-4o and Qwen-2 completing 22.8% and 26.0% of the harmful intents, respectively. Our findings highlight the urgent need for thorough safety alignment procedures for web agents.

## Which Harm Categories Are Agents Most Vulnerable Against?

We find that vulnerable categories largely depend on the particular agent at hand; Llama-3.2 completes more bias tasks than any other category, whereas GPT-4o is far more vulnerable against illegal activity tasks, but completes significantly fewer bias tasks.

<img src="/assets/tcr_radar_d-category_v2.jpg" width=500px>

## How Can I Use The Benchmark?

We make the benchmark, as well as all relevant code publicly available at (github.com/McGill-NLP/safearena)[https://github.com/McGill-NLP/safearena]; we also host the SafeArena (leaderboard)[https://huggingface.co/spaces/McGill-NLP/safearena-leaderboard]


