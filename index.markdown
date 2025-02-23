---
layout: default
---

<div align="center">

<h1>SafeArena</h1>
<h2>Evaluating Safety in Autonomous Web Agents</h2>

<i><strong>Ada Tur</strong> &nbsp; <strong>Nicholas Meade</strong> &nbsp; <strong>Xing Han Lù</strong> &nbsp; Alejandra Zambrano &nbsp; Arkil Patel &nbsp; Esin Durmus &nbsp; Spandana Gella &nbsp; Siva Reddy</i>

<strong>Equal Contribution</strong>

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

Overall Performance            |  Normalized Safety Score
:-----------------------------:|:-------------------------:
![](tcr_main_d-aggregate.jpg)  |  ![](tcr_main_d-normalized-safety.jpg)

We find that agents are surprisingly compliant with malicious requests, with GPT-4o and Qwen-2 completing 22.8% and 26.0% of the harmful intents, respectively. Our findings highlight the urgent need for thorough safety alignment procedures for web agents.


