---
layout: post
author: Andrew
title: Kanji Puzzle
categories: software-projects
---

Kanji Puzzle is an app idea that I am currently in the process of designing. 

[The proof of concept is now live!](http://kanjipuzzle.com/)

<figure class="float-right">
    <img loading="lazy" src="https://upload.wikimedia.org/wikipedia/commons/5/5c/It-%E5%AD%97.png" alt="It-字.png" width="60" height="60">
</figure>
<figure class="float-right">
    <img loading="lazy" src="https://upload.wikimedia.org/wikipedia/commons/3/3c/Han.png" alt="Han.png" width="62" height="60">
</figure>

Kanji are Chinese characters that are used in Japanese.

There are thousands of kanji characters, about 2000 are needed just to be at a high school reading level. The most common method of learning these characters is through pure memorization, with little or nothing else to go on. This method is crazy. It would be like trying to memorize the meaning of every word in the English dictionary without ever using any of those words in the definitions of other words.

Imagine trying to memorize the difference between 嬌 and 橋 through straight repetition. Then memorize a thousand other characters and still retain your memory of these two. If you break down the left part of each character though, you have the character for **woman** (女), and the character for **wood** (木). The right part of both characters is the same, and can be broken down further in a way that brings about the image of an **angel**. The first character’s meaning is **attractive** (woman + angel). Now memorizing the second character (**bridge**) is much easier, as bridges are made of **wood**.

This method of learning kanji was popularized by the book Heisig’s Remembering the Kanji, and is far more effective. But still, repetition and practice is involved as is with any other language or skill. Currently the way most people are practicing this method of learning is through the use of flash cards and writing. But Heisig himself states in his book, that with this method, repetitive writing is NOT the key to learning, the key is practicing this logical way of deducing the meaning of a character based on it’s components.

This is good news, as writing each character every single time you practice it is time consuming, and slows down the learning process. The ideal way to practice would be to piece each character together like a puzzle using smaller pieces that you already know how to write. There is currently no app that I have found that lets you practice this way, so I have decided to make it myself.

The mobile app is being developed in React Native. It will connect to a server API built with Ktor, and a postgresql database. 
