---
layout: post
title: New Website
---

As I started the process of thinking about my new site, I found it crucial to make a list of the requirements. This helps me focus on the bare minimum I need to achieve. Without this, the project can become open-ended and unending. I've found this out the hard way, as I unsuccessfully tried this activity in the past.

1. I want the site to be responsive, naturally. I will be designing it mobile-first. This means thinking about how it works on the smallest screen size first, then figure out how things flow, scale and position themselves as the screen gets larger.
2. I ~~want~~ need good typography.
3. At this point, I don't need more than 2 kinds of pages- those that are more image heavy (project showcases) and those that are more text heavy (writing). The same grid system must work for both cases. I won't spend too long on a creating a complicated grid system, since my needs are simple.

### Grid
I know that on small screens, all my columns are going to be full-width. As the screen becomes larger, the columns will then take up varying proportions of the screen real estate. If you are new to responsive design, Adam Kaplan has written an excellent guide to get you [started with the grid](http://www.adamkaplan.me/grid/) in responsive design.

Based on my requirements and some quick sketching, I decide that a 6 column grid gives me enough variation. I can combine columns to create two equal columns (3,3), three equal columns (2,2,2) or two unequal columns (2,4 or 4,2). Considering this, and not wanting to spend too much time on the grid, I decide to go with a this grid structure.

My next step is to figure out the column widths. At this point, I don't want to worry too much about huge screens, so I decide that I will use a `max-width` on my content area.

### Typography
Readability of body text is of great importance to me, so a good way to decide these column widths is to base them on the measure of your text. The 'measure' in typography is the line length of your body text. In *The Elements of Typographic Style*, Robert Bringhurst says that an acceptable measure for text set in a single column is 45-75 characters, including spaces. An ideal measure is 66 characters, so based on my chosen typeface, I want to get as close to this number as possible.

A confession: this part is not truly mobile-first design. This column width is going to be true for my larger screen sizes; fitting this many characters on mobile screens makes the text hard to read. Typecast has an excellent post about creating a [typographic scale for modern devices](http://typecast.com/blog/a-more-modern-scale-for-web-typography "A More Modern Scale for Web Typography"). On smaller screens, I'm going for around 35 characters per line. I am going to use their scale as a starting point for my typography, and tweak it from there.

I chose [Rooney Web Pro](http://www.janfromm.de/typefaces/rooney/web/) as my body copy typeface. At this point, I decided to take a gamble and see what happened with my 3 column grid at `max-width: 1024px;`. I used 30px padding on the left and right to create the gutters between columns. This gave me a `<p>` spanning 4 columns (two-thirds width) equalling 643px. Rooney Web Pro set at 19px gives me...68 characters per line on average! The text looks great at this size and I have my foundation set to move forward.

My next post will deal with setting up a Jekyll website from scratch, which I hope is useful to someone like me doing this for the first time.