---
title: How I use the Logseq Readwise plugin in my Zettelkasten
category: blog
format: article
showtoc: true
date: 2022-06-26
tags:
categories: blog
lastMod: 2022-06-26
---
![image.png](/assets/image_1656270634376_0.png)

The above image is the visualization of my Logseq graph, at least as of June 26th, 2022 at around 3:00 PM EDT. I know it's not as pretty or big as some others you may have seen, but I think it's a great way to see how I use Logseq, its linking capabilities, and its integrations.

You'll see some clusters there in the center. That represents the reference notes, topic tags, and main notes of my Zettelkasten. Some of the bigger nodes are reference notes because Logseq brings in the Zotero tags, and I create an author page for each. That messy web dead center is the majority of the main notes. I don't have enough to create super visible hubs, but it makes me happy that those notes don't create the "node with spokes" structure that the reference notes have.

Okay, so what are all the other notes floating aimlessly around the messy web? That's a great question.

Those are the highlights I've taken in various web articles and e-books as well as tweets and Twitter threads I've saved. They're brought in through the official Logseq Readwise plugin.

## What is Readwise?

Readwise is a read-it-later service which imports the highlights you take in other websites and apps. For example, any highlights you make in a Kindle book will be sent to Readwise. You can also manually enter highlights or take pictures of physical books to highlight. Once highlights are in Readwise, it prompts you every day to review highlights using spaced repetition.

## Why use Readwise?

I admit to having been skeptical when I first heard of Readwise. I'm not a student, and I don't feel the need to memorize stuff I read, *especially* when I'm reading for fun. The only reason I gave it a go was because I got a free annual subscription through the Building a Second Brain course I did. I started using it, and I liked it well enough to keep using it. It's fun to review highlights from books, web articles, and even tweets I haven't visited in a long time. Still, just revisiting highlights isn't meeting any need of mine, at least not one I would pay for.

However, what turned Readwise into a crucial part of my workflow is its ability to export highlights to other apps and services. In addition to reviewing highlights in the app every day, I also have those highlights in my note-taking apps to search and use. I used the Evernote integration for a while, but I don't really do thinking and creating work in Evernote. Evernote is my filing cabinet. I can full-text search and bring highlights up, but then I have to move those notes around, copy/paste, duplicate, whatever, if I want to use those exact quotations in something. I can't easily connect them to anything.

Then, I got brought on to test the official Logseq integration.

## Logseq Integration

I mentioned that I use Evernote as my filing cabinet in my "second brain." My other primary tool is Logseq. To quickly introduce it: Logseq is a free, open source outliner and note-taking program which prioritizes local files and privacy. It exists in the same type of app as Roam Research and Obsidian, which allow you to connect notes through backlinks. Logseq, like Roam Research, allows you to reference and embed at the "block" level, not just the page level.

The ability to reference/embed at the block level is what makes Logseq work so well with Readwise. For example, one thing I love about Readwise is that it can save Twitter threads. I used to hate bookmarking the first tweet in a thread, or even bookmarking every single tweet in the thread. In Readwise, I can find that thread and review it, but the individual tweets will be split when doing a daily review. I often review tweets out of context with the rest of their thread. In Logseq, however, Readwise creates a new page for each larger work a highlight is in –– a page for each book you have highlights in, for each article you have highlights in, etc. And for twitter threads, it creates a page for that entire thread.

And each individual highlight has its own block on that page, allowing me to embed and reference it when needed. The highlights don't exist out of context of their larger work, but I can still use them individually *in a way that is linked back to the larger context*.

![Tweet highlights in Logseq](/assets/Screen-Recording-2022-06-26-at-1_1656264513852_0.gif)

The integration also creates page links for the author of the larger work and the category (but I remove the category link). It brings in any tags you've made in Readwise for the larger work and the individual highlights and any notes you've made for each highlight. Finally, it provides external links to the original source if applicable, including links to individual tweets and Kindle locations.

## My configuration

Before I walk you through the parts of my workflow which include Readwise, I want to explain my setup and configuration. My setup is not complicated, but it is not the default, either.

There are several options to configure. For example, you can automatically sync new highlights when you open Logseq. I don't do this because highlights are only as good as their original page metadata, and I often have to change authors in Readwise. For Logseq in particular, I have to make sure titles don't contain forward slashes because forward slashes will create namespaces. Disabling autosync gives me time to clean up any metadata before I bring it into my graph. You can also choose to resync deleted pages. I turn this on when I notice some bad metadata or formatting that needs fixing, but I don't have it on as the default.

![Screen Shot 2022-06-26 at 2.01.43 PM.png](/assets/screen_shot_2022-06-26_at_2.01.43_pm_1656266525073_0.png)

When you click "Customize" for formatting options, you have several more options to configure. I choose to leave on "Include Highlight Location," and I turn on "Use Custom Formatting."

![Screen Shot 2022-06-26 at 2.02.48 PM.png](/assets/screen_shot_2022-06-26_at_2.02.48_pm_1656266587784_0.png)

When you turn on Custom Formatting, you can change the template Readwise uses to create your highlights pages.

The first is the page title. I am fine with the default because having `(highlights)` in the title provides an easy way to search and filter without creating a giant page node in my graph.

![image.png](/assets/image_1656266727175_0.png)

Then we have page metadata. I change the default in two ways. The first is that I put quotation marks around the full title value. Otherwise, multiple pages will be created if the title has a comma in it. However, this default may have changed by time of publication or sometime after. I also remove the tag from category. I don't want a giant cluster in my graph, and I don't need to see every source I have that's a book. Some people might, though! This is just my preference.

![image.png](/assets/image_1656266754887_0.png)

Readwise creates a header to nest highlights under. I remove the backlinks from where it says Readwise because I don't want a giant page node in my graph view. That is a connection that isn't useful to me, but it might be for you.

![image.png](/assets/image_1656266945184_0.png)

For the actual highlight, I don't change anything. I would like to make the Tags a block property, but I'm not skilled enough to figure that out. I edit as needed.

![image.png](/assets/image_1656267108646_0.png)

Finally, there's the sync notification. Because I haven't created a Readwise page in the highlights header, there's no place for this notification text to go. I just leave it as the default.

And, like with other Readwise exports, you can choose to select specific items or sync everything.

## Workflow

I use Logseq as my digital [Zettelkasten]({{< ref "Zettelkasten" >}}), and my workflow is fairly traditional. With a focus on how Readwise fits in, here's what it looks like:

I'm reading an e-book, an online article or blog, or tweets; I don't use Readwise for scholarly articles which I have as PDFs. I make highlights related to a current interest of mine, either because I'm reading for that interest or because I notice something that relates even when reading for fun.

When reviewing highlights, I'll add topic tags and notes as appropriate. After making sure all the metadata and formatting is cleaned up (seriously, remove the markdown footnotes if you highlight Wikipedia articles), I sync those highlights in Logseq to create pages. **The pages generated by Readwise now become one part of an eventual reference (or literature) note.**

![Screen Shot 2022-06-26 at 3.29.36 PM.png](/assets/Screen_Shot_2022-06-26_at_3.29.36_PM_1656271798423_0.png)

I have some fleeting notes, and I decide to make a Zettel (or main note) out of one. Because what I want to say is usually *in response* to something else, I like to make a reference note for that something else. If the source is not already in my Zotero library, I add it. Then, I make a page for that reference in Logseq via the Zotero integration. If I also have Readwise highlights for that reference, I put a page reference in the reference note to the highlights page.

![Screen Shot 2022-06-26 at 3.13.58 PM.png](/assets/Screen_Shot_2022-06-26_at_3.13.58_PM_1656270872003_0.png)

Now, when I write my Zettel, I can cite my source by linking to my reference note.

![Screen Shot 2022-06-26 at 3.24.06 PM.png](/assets/Screen_Shot_2022-06-26_at_3.24.06_PM_1656271502787_0.png)

I don't link to the Readwise highlights page, but because that page is linked in my reference note, a link is created between it and my main note I've just written. I can also do block references with specific highlights I want to use as quotations. However, I don't do this because I publish my Zettelkasten online, and it can only handle block references to other pages I've published; I don't put my Readwise highlights or reference notes online. There is a Logseq plugin which allows you to swap a block reference and a block, but when I've tried it in this workflow, the block id gets included in the Hugo-compatible Markdown.

And honestly, that's pretty much the main workflow!

## Other uses

I do not makes notes of everything I read, watch, or listen to just for the sake of making notes. But a nice thing about having my captured highlights in Logseq is seeing how clusters form, generatively, without me necessarily having done anything.

Let me explain.

Like how the Zotero integration brings in tags, so too does the Readwise integration. This includes the hashtags in tweets, in addition to whatever tags I've added to a highlight. The giant cluster at the top of my graph isn't any sort of "main note" cluster at all: it's a cluster of Readwise highlights linked to the page "art." It's so big because a lot of tweets I send to Readwise that have art in them have the hashtag "art."

Sometimes, I will review highlights to see what tags or notes I might add. I use the Logseq Random Note plugin for that, and because so many of my Logseq pages are actually from Readwise, a lot of the notes I see when using the Random Note plugin are Readwise highlights.

I don't tag every note that comes up. Just like when I'm reading, I only try to add tags or notes that are relevant to a current interest of mine. I don't need to tag [this incredible tweet of David Duchovny on Celebrity Jeopardy](https://twitter.com/yacobg42/status/1325500299440754690?s=20&t=gT9ckEjkcf-jc8eLEjqpUg) with "frogs" or "X-Files." But if I see something that is related to a topic, I'll tag it or add a related existing page.

![Screen Shot 2022-06-26 at 3.58.32 PM.png](/assets/screen_shot_2022-06-26_at_3.58.32_pm_1656273551693_0.png)

-----

I'm beyond excited to see where the Logseq Readwise plugin goes. I love it so much as is, and it's only just starting. I think Logseq and other tools which include block references are a perfect match for Readwise. It's so nice to be able to link to or embed individual highlights without those highlights having to be on their own pages out of context.

I am also not someone who thinks we need to do something with every bit of information we interact with; I get exhausted just thinking about the people who write huge book summary reading notes for every single thing they read. But having Readwise highlights in Logseq allows me to add notes, tags, and links to highlights as needed. Plus, Logseq's "Unlinked References" section and the Random Note plugin can create moments of serendipitous discovery.

And that's how note-taking and personal information management should be: serendipitous and fun.

## Shameless plug time

To whoever reads this: I would love to hear about your workflows, especially if you use Zotero.

If you're curious about using Zotero in a workflow which includes the Readwise integration, I offer coaching, mentoring, and consultation for Zotero in personal information management. Don't hesitate to reach out to me: https://linktr.ee/jlcolbert
