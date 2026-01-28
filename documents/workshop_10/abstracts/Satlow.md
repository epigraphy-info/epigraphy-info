---
layout: abstract
title: "Using AI to Encode Inscriptions"
authors: "Michael Satlow (Brown University)"
---

## Abstract
This paper will present the results of research that sought to use AI technologies to encode ancient, multilingual inscriptions. “Inscriptions of Israel/Palestine” (inscriptionsisraelpalestine.org) has always used human encoders to enter our inscriptions, which are in Greek, Latin, Aramaic, and Hebrew. This involves converting inconsistent publication data into an XML document that accords with our tailored version of an EpiDoc schema. The process is time consuming (30 minutes to an hour per inscription), especially the translation of conventional Leiden typography to our own tags. Current automated approaches, which rely on using regular expressions, were surprisingly inconsistent. We thus experimented to see if LLMs could do a better job.

We produced a pipeline, using the AI client Claude, that can do this translation with a good degree of accuracy. This presentation will describe that pipeline and our metrics and evaluation criteria. We have developed an app that can do this work, and we will describe how that app can be used and tailored for different tag sets. Finally, we will also describe our (so-far failed) experiments in designing a more comprehensive pipeline that can move
from a pdf to a fully formed XML file that includes both the tagged inscription and its metadata.

---  
[Back to Day 1 programme]({{ site.baseurl }}/workshop_10/#day-1)