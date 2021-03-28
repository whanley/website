---
title: "Egypt's cabinets in Wikidata"
date: 2020-11-18
description: "Documenting upload of Egyptian minister data to Wikidata."
type: "post"
image: "images/1939-cabinet.jpg"
categories:
  - "Computational methods"
tags:
  - "Wikidata"
  - "OpenRefine"
  - "Egypt"
---

***

I am a hater of Wikipedia haters. It drives me up the wall when my kids' history teachers ban them from using it. I use it all the time, even for topics I pretend to have mastered.

## Horsing around with Wikipedia
I'm writing a book about international law in Cairo. One chapter is a study of a huge probate case (Antun Yusuf 'Abd al-Messih) that began in 1885. As I was investigating the background of Antun's debtors, I started reading about Ali Pasha Sherif, whose luxury lifestyle was funded by loans of up to £100,000. I remembered Ali Pasha as one of the slaveholding elites described in Eve Troutt Powell's 2003 [A Different Shade of Colonialism](https://www.ucpress.edu/book/9780520233171/a-different-shade-of-colonialism).

Computational methods are key to my work on this book. I'm trying (so far without great success) to describe the basic producers of the wealth that fueled litigation of the sort that I'm examining. To that end, I'm working to tie all my datasets into [Wikidata](www.wikidata.org), which is the leading [linked data](https://en.wikipedia.org/wiki/Linked_data) hub. Wikidata is fuelled in part by Wikipedia, and I was pleased to see that Ali Pasha has an [entry](https://en.wikipedia.org/wiki/Ali_Pasha_Sherif).

Like many entries about Middle East topics, it's quixotic. Its [earliest iteration](https://en.wikipedia.org/w/index.php?title=Ali_Pasha_Sherif&oldid=94585857) is a paraphrase of a [page](https://web.archive.org/web/20050324020615/http://members.aol.com/NadaraDefs/WebPage/AliPashaSherif.html) from an old [AOL site](https://web.archive.org/web/20050206170300/http://members.aol.com/NadaraArab/) by a California enthusiast of "Egyptian Arabian Sport Horses." Not surprisingly, it has more to say about Ali's horses than the man himself. But it said that he was Egypt's foreign minister; of course I immediately thrilled to the idea of international legal precedent established by the personal debts of a colonized foreign secretary.

To the credit of my kids' history teachers, Wikipedia *was* wrong: Ali Pasha was never Egypt's minister (though his brother _was_ Ottoman foreign minister). To my credit, Wikipedia is no longer wrong: I corrected the error and tidied up the page. Thanks to the enthusiast who produced the original text, I learned some things about the Egyptian horse market in the 1870s and 80s, and I came better to understand Ali's debts to Antun. And as I tried to figure out who had and had not been Egypt's foreign minister, I discovered another enthusiast: [عادل](https://ar.wikipedia.org/wiki/%D9%85%D8%B3%D8%AA%D8%AE%D8%AF%D9%85:%D8%B9%D8%A7%D8%AF%D9%84), who has made [thousands and thousands and thousands of contributions to Arabic wikipedia](https://ar.wikipedia.org/w/index.php?title=%D8%AE%D8%A7%D8%B5:%D9%85%D8%B3%D8%A7%D9%87%D9%85%D8%A7%D8%AA/%D8%B9%D8%A7%D8%AF%D9%84&offset=&limit=500&target=%D8%B9%D8%A7%D8%AF%D9%84), including an incredible set of pages listing [Egyptian Ministers](https://ar.wikipedia.org/wiki/%D8%AA%D8%B5%D9%86%D9%8A%D9%81:%D9%82%D9%88%D8%A7%D8%A6%D9%85_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D8%A7%D9%84%D8%AD%D9%83%D9%88%D9%85%D8%A7%D8%AA_%D8%A7%D9%84%D9%85%D8%B5%D8%B1%D9%8A%D8%A9), among them a complete page on the [foreign ministers](https://ar.wikipedia.org/wiki/%D9%82%D8%A7%D8%A6%D9%85%D8%A9_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D8%A7%D9%84%D8%AE%D8%A7%D8%B1%D8%AC%D9%8A%D8%A9_(%D9%85%D8%B5%D8%B1)).

## Listing foreign ministers
In a burst of enthusiasm, I got down to work replicating Adil's Arabic ministers list in English. [I made it to 1930](https://en.wikipedia.org/wiki/Minister_of_Foreign_Affairs_(Egypt)) before I ran out of steam. I was worn down by a few factors:
- my own desire to move on to the next thing before finishing the task at hand
- [MediaWiki's table syntax](https://www.mediawiki.org/wiki/Help:Tables), which is a bit intricate to do by hand (I realize now I should just have used a [convertor](https://commons.wikimedia.org/wiki/Commons:Convert_tables_and_charts_to_wiki_code_or_image_files))
- missing Wikipedia entries for many of the foreign ministers of Egypt (the topic of the rest of this section)
- a sense that I should fill out this dataset in a more portable format (which is the topic of the rest of this post)

Wikipedia entries on Middle East topics are a treasure trove of resources, especially if you work your way through the "Languages" links at the bottom of the left hand menu. The foreign ministers list looks very different in [English](https://en.wikipedia.org/wiki/Minister_of_Foreign_Affairs_(Egypt)), [Arabic](https://ar.wikipedia.org/wiki/%D9%82%D8%A7%D8%A6%D9%85%D8%A9_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D8%A7%D9%84%D8%AE%D8%A7%D8%B1%D8%AC%D9%8A%D8%A9_(%D9%85%D8%B5%D8%B1)), and [German](https://de.wikipedia.org/wiki/Liste_der_Au%C3%9Fenminister_%C3%84gyptens). The [Persian version](https://fa.wikipedia.org/wiki/%D9%88%D8%B2%DB%8C%D8%B1%D8%A7%D9%86_%D8%A7%D9%85%D9%88%D8%B1_%D8%AE%D8%A7%D8%B1%D8%AC%D9%87_%D9%85%D8%B5%D8%B1) is based on the Arabic page [before Adil upgraded it](https://ar.wikipedia.org/w/index.php?title=%D9%82%D8%A7%D8%A6%D9%85%D8%A9_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D8%A7%D9%84%D8%AE%D8%A7%D8%B1%D8%AC%D9%8A%D8%A9_(%D9%85%D8%B5%D8%B1)&oldid=45703967), while the [Russian version](https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BC%D0%B8%D0%BD%D0%B8%D1%81%D1%82%D1%80%D0%BE%D0%B2_%D0%B8%D0%BD%D0%BE%D1%81%D1%82%D1%80%D0%B0%D0%BD%D0%BD%D1%8B%D1%85_%D0%B4%D0%B5%D0%BB_%D0%95%D0%B3%D0%B8%D0%BF%D1%82%D0%B0) appears to be its own animal. Considering the importance of Egypt to France (and vice versa), it's remarkable that there is no French page.

As I worked to mirror the Arabic list in English, I found that several ministers had Arabic pages without English counterparts. I made brief, rough [stub](https://en.wikipedia.org/wiki/Wikipedia:Stub) pages for

* [Wasif Boutros Ghali](https://en.wikipedia.org/wiki/Wasif_Boutros_Ghali)
* [Ali Zulfikar Pasha](https://en.wikipedia.org/wiki/Ali_Zulfikar_Pasha)
* [Tigrane Pasha](https://en.wikipedia.org/wiki/Tigrane_Pasha)
* [Nakhla George al-Motyei Pasha](https://en.wikipedia.org/wiki/Nakhla_George_al-Motyei_Pasha)

None of these is great work, but they're enough for others to build out if and when they feel the need.

As is often the case, the fine folks who volunteer to keep Wikipedia tidy were [cautious to accept thinly referenced new entries](https://en.wikipedia.org/wiki/User_talk:Will_Hanley#Ways_to_improve_Tigrane_Pasha). Their position is reasonable enough. At the same time, the effort to expand Wikipedia beyond dead white men sometimes founders on the lack of easily accessible, English-language secondary sources. Wikipedia editors tend to reflexively expect reference to such sources to verify [notability](https://en.wikipedia.org/wiki/Wikipedia:Notability). It's easy enough when there's a _Times_ obituary (as there is for Tigrane Pasha). It's more difficult if you build your page entirely on a paragraph in [Zirikli](https://en.wikipedia.org/wiki/Al-Zirikli)'s *al-A'lam*, which is what I usually do.

Things get easier when there's an entry in Arabic wikipedia that you can mirror. Best of all is if the subject is an author who can be found in [VIAF: The Virtual International Authority File](viaf.org) and [WorldCat](https://www.worldcat.org/identities/). Linking to those [authority controls](https://en.wikipedia.org/wiki/Wikipedia:Authority_control) usually makes the case for notability clear. In addition, these catalogues provide an easy list of books to add to the Wikipedia entry.

It takes a bit of time to make a new page, however, and there were dozens of such pages required to fill out the list of Egypt's foreign ministers. Many of these men were less notable, and I didn't feel up to doing the digging.

## Closed versus open formats
While I was searching up the lesser-known names on the list, I came across another amazing Wikipedia contribution from Adil: in 2016 he created a page for [every Egyptian cabinet ](https://ar.wikipedia.org/wiki/%D8%AA%D8%B5%D9%86%D9%8A%D9%81:%D9%85%D8%AC%D8%A7%D9%84%D8%B3_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D9%85%D8%B5%D8%B1%D9%8A%D8%A9) from 1878 to the present. Our brilliant friend produced tables listing every minister and ministry. He drew his information from encyclopedic works by [Mohammad al-Gawadi](https://ar.wikipedia.org/wiki/%D9%85%D8%AD%D9%85%D8%AF_%D8%A7%D9%84%D8%AC%D9%88%D8%A7%D8%AF%D9%8A), [Younan Labib Rizk](https://www.worldcat.org/identities/lccn-n82268090/), and others, and he cites these sources scrupulously.

When I saw these lists, I thought that I could approach this problem differently. Instead of spending a month writing Wikipedia pages, I could spend a few days converting these well-formatted and standardized tables into a format that I could upload to Wikidata.

What is the difference between Wikipedia and Wikidata? Wikipedia is written by and for human readers. While there are automatic bots that crawl through the pages to standardize spelling and dates and categorize pages, almost all of the work is done "by hand." Wikidata, on the other hand, is written for and (to a large extent) by automatic readers. It is an elaborately structured dataset based on a fascinating category structure (or [ontology](https://en.wikipedia.org/wiki/Ontology_(information_science))) that attempts to describe all existence.

I won't bore the few readers who have made it this far with rhapsodies about Wikidata. Suffice it to say that this dataset nourishes all sorts of automated reasoning about our world. Those committed to combatting Eurocentrism do well to contribute data to this pool, which tilts very, very white, male, and wealthy. Egyptian ministerial data is not the ideal remedy for that problem. It is an improvement on what's there, however. Even more important, any information that is already digitized, cleaned, and structured is fairly easy to upload. And so that's what I resolved to do.

This undertaking is not purely altruistic. I expect to be able to use it to support my own research as well. Wikidata has a [query service](https://query.wikidata.org/) that uses the powerful [SPARQL](https://en.wikipedia.org/wiki/SPARQL) language. It's fun for trivia: here's a query for the [first names of everyone (for whom a first name and birthplace is recorded) who was born in Cairo](https://w.wiki/k8S) (press play to get it to run). It can also be fun for more serious questions, so long as the dataset is relatively complete. That's what I set out to do with the ministers.

## Documenting the process
The next part of this post is fairly dry. I'm recording details so that others searching for a "how to" can learn from my attempts, and so that I can remember what I did. If you're not interested in the step-by-step, I urge you to jump to the end.

### Preparing the data for OpenRefine

1. Copy table contents from [Arabic foreign ministers pages](https://ar.wikipedia.org/wiki/%D9%82%D8%A7%D8%A6%D9%85%D8%A9_%D9%88%D8%B2%D8%B1%D8%A7%D8%A1_%D8%A7%D9%84%D8%AE%D8%A7%D8%B1%D8%AC%D9%8A%D8%A9_\(%D9%85%D8%B5%D8%B1\)). It would be possible to automate this, but I did it manually in fifteen minutes.
2. Paste tables into spreadsheet, figure out odd parts (mostly having to do with post-1952, when there were frequent prime minister changes but few minister changes), then paste results into plain text editor as tab separated values. Keep working till you have one line per ministry.
3. Create new table in OpenRefine.
4. Parse dates in OpenRefine until they are standardized. The easiest way to do this is to split the date into several columns (by space). Then
5. Reconcile Prime Minister names with Wikidata. This is easy, because they're already there.
6. Make a new column by fetching English labels (Property Len). Add "Cabinet" to the end. Fill down.
7. Filter wizara column by ordinal numbers (al-ula, etc), then add English equivalent to Cabinet column.
8. Some foreign ministers' terms cover two cabinets. Filter for these, clean up end dates, etc, then delete the excess rows.
9. Reconcile Arabic cabinet names against Wikidata. Straightforward enough, because they are already there from the Wikipedia pages, but they are empty.
10. Add description, using "Egyptian government formed in " plus year in start column.
11. Add head of state column, manually with khedives, reconcile, then fill down.
12. Add follows, followed by, reconcile.
13. Map to schema.

1. Cut and paste all of the cabinet tables from the various cabinet pages, in sequence, into spreadsheet.
2. Filter for prime Minsters, Add column with them.
3. Match them with their cabinets (by hand)

**Note**: Image from [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:King_Farouk_and_Aly_Maher_2nd_Cabinet_1939.jpg)
