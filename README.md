# How to use

## -1- Generate a TOC

Switch to "author" mode in droplist for GHCP and type something like 

```
generate a TOC on [topic].
```

The more context you give here the better, example "Generate TOC on javascript and Azure AI Foundry, should be for beginners, max 15 chapters"

.github/chatmodes/author.chatmode.md will take care of the rest to add key concepts and more.

## -2- Generate a chapter

Once you have a TOC, you can type the following in the chat (switch out the chapter number as needed):

```text
Generate chapter <chapter_number> according to TOC.md, you must follow your chosen chat mode and writing guidelines, this is non negotiable
```

This should create a chapter using BOOK.md as guidelines and create a chapter under chapters/<chapter_number-title>.md.

##  -2b - Generate a blog post

```text
Generate a blog post on <topic>, you must follow your chosen chat mode and writing guidelines, this is non negotiable
```

This creates a very comprehensive blog post. For shorter posts use the following prompt instead:

```text
Generate a 5 min read blog post on <topic>, make it engaging and beginner friendly, you must follow your chosen chat mode and writing guidelines, this is non negotiable.
```

This should create a blog post using BLOG.md as guidelines and create a blog post under posts/<date-topic>.md

## -2C- Generate video scripts

```text
 see here, https://learn.microsoft.com/en-us/training/support/mcp now create video script based on the scenario I gave you "How to add postgres database to app and how that's made easier as microsoft learn mcp server helps you look up docs from vs code"
```



## -3 Review chapter

NOTE: most of the time the author mode does a fantastic job so you might not even need to run this one.

Switch to "reviewer" mode in droplist for GHCP

Type the following in the chat (switch out the chapter number as needed):

```text
Review Chapter 1
```

## Finally

NOTE: the prompts above are probably more detailed than you need, but they are designed to ensure the writing guidelines are followed, which is critical for quality.

Finally, enjoy your new chapter or blog post!
