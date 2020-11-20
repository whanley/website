---
title: "Pashas into Wikidata"
date: 2020-11-18
description: "Seven step-by-step videos documenting conversion and upload of a list of Egyptian notables."
type: "post"
image: "images/fez.jpg"
categories:
  - "Computational methods"
tags:
  - "Wikidata"
  - "OpenRefine"
  - "Egypt"
---

I am experimenting with [Wikidata](http://wikidata.org) as a research data repository. If I systematically upload various datasets, can I a) make wikidata more global and useful, and b) learn more about my own evidence?

I documented two recent projects, in two different ways. I wrote a [step-by-step text description of my work to put Egyptian ministers into Wikidata](2020-11-18-cabinet-to-wikidata). In that post, I outline my reasoning in greater detail and offer some useful links about the process.

Here, I want to share screen capture videos of my work to put Egyptian pashas into Wikidata. The videos, in sequence below, are soporifically self-explanatory. I haven't done documentation like this before, and it was fun. I'm shocked at how much time I can spend talking about this stuff.

### 1. Wikipedia to OpenRefine

In the first video, I take a list of 353 Egyptian men given the title "pasha" between 1910 and 1952, from [this Arabic wikipedia page](https://ar.wikipedia.org/wiki/%D9%82%D8%A7%D8%A6%D9%85%D8%A9_%D8%A8%D8%A7%D8%B4%D9%88%D8%A7%D8%AA_%D9%85%D8%B5%D8%B1), and begin to tidy it in [OpenRefine](https://openrefine.org/).

{{< youtube PflmQn_SFbg >}}

### 2. Dates

Here I change the dates of appointment into YYYY-MM-DD format.

{{< youtube wFmEePPYY_Y >}}

### 3. Given names

Here I add a column containing each pasha's given name.

{{< youtube fonr9Su4ZhQ >}}

### 4. Wikidata reconciliation

Here I find how many of these fellows are already in Wikidata. For those already present, I will only want to update their records to add the title "pasha" and the date. For those men not yet in Wikidata, I will want to create a whole new item.

{{< youtube WUgO8Tkhu6s >}}

### 5. Adding data from a second source

Here I start to incorporate a [different list](http://www.egy.com/historica/pashalst.php), which gives the same information in English, from Samir Rafaat's redoubtable [egy.com](http://www.egy.com).

{{< youtube T30k1AzLc6Q >}}

### 6. Combining Arabic and English lists

Here I explain how I brought together the Arabic and English lists. I don't think I did this in a very efficient manner, but so it goes. I considered it worth some effort to add these English transliterations, because they will really enrich the Wikidata items.

{{< youtube JXlHWUhowxw >}}

### 7. Wikidata schema

My OpenRefine file is clean, consistent, and complete. In this video I map it to a Wikidata schema, which describes the kind of information that I want to upload. Then I upload the material.

{{< youtube hty7PJRabQg >}}

### 8. Querying Wikidata

Here I will upload a video showing how this pasha data can be used once it's in Wikidata.

**Note**: The image of a Shriner's hat from Tampa, Florida is pilfered without permission from [pinterest](https://www.pinterest.com/pin/265642077999094699/), but I excused myself because Orientalism.
