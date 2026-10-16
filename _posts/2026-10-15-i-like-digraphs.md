---
layout: post
title: "Simple minds find simple joys"
tags: [vim]
context: [digraph, i_CTRL-K]
date: 2026-10-15
---

Given that hundreds of thousands of people could be reading this blog already,
I suppose that it is conceivable that there are a few of you out there who are
unfamiliar with digraphs. I wouldn't want to burden you with the trouble of Googling it (a
term which I have been informed by the younger generation is no longer
relevant), so suffice to say it is an old Greek word that means two characters
that make a single sound. 

In Vim, a digraph is taken to be a character outside of our regular keyboard-ascii-reachable range composed of two characters which are in our keyboard-ascii-reachable range.
If you are a self loathing patriotism lacking Canadian who uses the EN-US keyboard mapping instead of the EN-CA like myself, it may be helpful to know that with `<C-k>e'` you can be the pretentious diva you really are and tell people that you didn't have a coffee, but instead a *Caffé Americano*.

The digraph in particular that inspired me to write about this is `→`. I had been looking into a font pack that supported
ligeratures in a previous post for converting "->" to "→" when it dawned on me that I had a far simpler solution in my arsenal. I smacked that
`i` for insert mode, I rolled my `<C-k>` and when my fingers typed ->, I didn't even need to look at the screen to know it had worked. A stupid smile crept onto my face.

In that moment, I was one with Vim.

Then this morning, I — a carbon based life form — actually needed to employ an em-dash.
I closed my eyes and confidently typed `<C-k>em`. I'm not sure if it was to my dismay or if it was to my chagrin,
but when I opened my eyes I was face-to-face with め. I know not from which alphabet nor
language that symbol is derived from, but I am quite confident in my assumption that
it loosely translates to "Failure".

I had lost touch with Vim, I had fallen from grace.

There was no time to dwell on this defeat, I still needed an em-dash. I begrudingly opened up `:digraphs` and began looking for the real McCoy,
only to realize that searching for a character that isn't even on your keyboard is an excerise in futility and a hobby reserved for sadists.

Maybe the kids will judge me for saying so, but I wasted no time and just
*Googled it*, and you better believe I got exactly what I was looking for:
`<C-k>-M`. Now, given that I don't particularly like that mapping, I decided to
exercise my freedoms and ran `:digraph em 8212` (The 8212 I got from doing `ga`
in normal mode on the em-dash). 

After performing this black magic, I felt like I was becoming one with Vim again. Under a new paradigm, one of
understanding that I wasn't built to become Vim, but that Vim was built to become me, and that I am `<C-k>em = —`,
and now Vim is too.
