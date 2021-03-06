---
author: dfwu
comments: true
date: 2019-04-13 14:15:44+00:00
layout: post
link: https://dfwu.wordpress.com/2019/04/13/this-is-my-first-post/
slug: this-is-my-first-post
title: What is Wrap-XP and why I think it is wrong
wordpress_id: 16
categories:
- Prosody
---

Wrap-XP is an important and influential notion in prosody (the study of how sounds in a sentence are grouped together). In this blog post I will explain what Wrap-XP is and why I think it is wrong.
<!-- more -->

  
Wrap-XP was first proposed in [Truckenbrodt's dissertation](http://www.ai.mit.edu/projects/dm/theses/truckenbrodt95.pdf) as a constraint in the sense of Optimality Theory[.](http://www.ai.mit.edu/projects/dm/theses/truckenbrodt95.pdf) As language creates prosodic structure from syntax, Wrap-XP requires a certain type of syntactic phrases (call them _type-A syntactic phrases_ for now) not to be broken up by any prosodic phrase (ф) boundary. In other words, for every type-A phrase, we must be able to find a ф such that the type-A phrase is not broken up in this ф. Crucially, Truckenbrodt argues that Wrap-XP only cares about type-A phrases, but not other kinds of phrases (let us call the complement of type-A phrases _type-B syntactic phrases_). Therefore, only type-A phrases may not be broken up by ф, but type-B phrases can be broken up by ф.  
To give you an example of how Wrap-XP works, suppose that a type-A phrase AP contains two phrases XP1 and XP2 in syntax: [XP1 XP2]. In mapping from syntax to prosody, imagine we want to create a prosodic phrase ф for each syntactic phrase. We may create a ф for XP1 and a ф for XP2: (XP1)(XP2).[1] Wrap-XP does not like this prosodic structure because the AP, which contains XP1 and XP2, is broken up by the prosodic boundary between XP1 and XP2. If we prefer to satisfy Wrap-XP, then we will need to remove the boundary between XP1 and XP2 and generate (XP1 XP2).  
But if it is a type-B phrase BP that embeds XP1 and XP2, then Wrap-XP does not care if this BP is broken up and will allow this structure: (XP1)(XP2).  
Here is the flaw of Wrap-XP: every time a type-A phrase contains a type-B phrase, we run into problems. First, consider a sentence with only a type-B phrase that contains XP1 and XP2. Wrap-XP does not care whether the type-B phrase is broken up by a prosodic boundary, and so we create boundaries between XP1 and XP2: (XP1)(XP2).  
Next, consider another utterance where this BP is embedded in an AP. Then Wrap-XP cares about this AP and requires no subdivision within it. Thus, all the boundaries we created earlier within the BP have to be removed: (XP1 XP2).  
Basically Wrap-XP says: depending on what the highest embedding phrase is, there may or may not be subdivision within this phrase. If we have a type-A phrase embedding a type-B phrase, we have to erase all the phrasing created earlier in the type-B phrase. This can't be right.  
Any attempt to revise Wrap-XP won't work either. As long as Wrap-XP discriminates, i.e. it only applies to some types of syntactic phrases but not others, the same problem will occur every time a phrase it applies to embeds a phrase it doesn't apply to.   
Now I will explain why Wrap-XP must discriminate. If Wrap-XP does not discriminate, it just means that all the utterances cannot be broken up by any prosodic boundary. This is not what we see in the languages where Wrap-XP was argued to be relevant.  
Truckenbrodt argues that Wrap-XP is relevant in at least two languages, Papago and Chichewa. In Papago, any syntactic phrase to the left of the tense head must have its own corresponding ф, while any syntactically phrase between the tense head and the verb head is grouped with the verb prosodically. The prosodic phrasing looks like this: (XP1)(T XP2 XP3 V). In Chichewa, subjects in Spec, TP always have their corresponding ф too.   
These facts lead Truckenbrodt to propose a discriminating Wrap-XP. In Papago, Wrap-XP should apply to the phrase that immediately dominates T, XP2, XP3 and V, but not to the phrase that immediately dominates XP1. Likewise, in Chichewa Wrap-XP should apply everywhere except to the phrase that immediately dominates the subject. 





[1]: One may wonder why ((XP1)(XP2)) isn't a possible structure for an AP embedding XP1 and XP2 [AP XP1 XP2]. If it is, then Wrap-XP is always satisfied because AP is not broken up in the largest ф. The prosodic structure where a ф contains another ф is called a recursive structure. For many years researchers believed that recursive structure is not allowed in any language. Since Truckenbrodt's dissertation, some have changed their view and thought that some languages may allow recursive structure, while other languages don't. Crucially, Truckenbrodt has argued on independent grounds that Papago and Chichewa don't allow recursive structure, so Wrap-XP would still run into problems in those languages, or any language that doesn't allow recursive prosodic structures.





 
