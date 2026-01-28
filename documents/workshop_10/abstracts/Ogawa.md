---
layout: abstract
title: "Evaluating Large Language Models for Automatic Generation of EpiDoc
TEI from Leiden Transcriptions"
authors: "Jun Ogawa (The University of Tokyo)"
---

## Abstract

This study addresses the trade-off in Latin epigraphic databases between fine-grained structured data and large-scale coverage. While EDH provides highly structured TEI/XML, its corpus remains limited, whereas EDCS offers far broader coverage but lacks consistent structuring. To mitigate this gap, the
project explores converting EDCS transcriptions into EDH-compatible EpiDoc using LLMs. 

The main focus is an evaluation of LLMs’ ability to transform Leiden-style transcriptions into valid EpiDoc XML. Pairs of transcriptions and ground-truth EpiDoc files from EDH were used to test three models—GPT-5, Gemini 2.5 Flash, and Claude 4 Sonnet—under two prompting conditions: (1) minimal instruction with only a link to the EpiDoc Guidelines, and (2) detailed instruction including sample transcriptions and markup examples. Outputs were validated by a rule-based script and assessed using three weighted metrics: Structural Match (30%), Content Match (50%), and Attribute Match (20%).

Results out of nine inscriptions found at the African city of Uthina indicate that GPT-5 performs best overall, particularly in structural understanding. Claude 4 Sonnet shows strong content-level performance but unstable behavior, such as adding quotation marks or header string outside the main XML body despite being instructed to output only XML elements (see Claude-4-Sonnet, ‘without instruction’). Detailed prompting significantly improves Attribute Match across models, demonstrating that explicit instruction is crucial for producing correct XML attribute values.

While promising, as the evaluation depends solely on EDH, and transcription practices sometimes differ between EDH and EDCS, further methodological refinement is required for reliable large-scale automatic EpiDoc generation using LLMs.

---  
[Back to Day 1 programme]({{ site.baseurl }}/workshop_10/#day-1-march-24)