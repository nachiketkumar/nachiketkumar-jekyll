## Requirements

As I start the process of thinking about my new site, it is useful to make a list of the requirements:

1. I want the site to be responsive, naturally. I will be designing it mobile-first. This means thinking about how it works on the smallest screen size first, then figure out how things flow, scale and position themselves as the screen gets larger.
2. At this point, I don't think I'll need more than 2 kinds of pages- those that are more image heavy (project showcases) and those that are more text heavy (writing/blog). The same grid system must work for both needs.
3. I don't want to spend too long on a creating a complicated grid system, because my needs are simple.

### Grid
I know that on small screens, all my columns are going to be full-width. As the screen becomes larger, the columns will then take up varying proportions of the screen real estate. If you are new to responsive design, Adam Kaplan has written an excellent primer to help you [understand the grid system](http://www.adamkaplan.me/grid/) in this respect.

Based on my requirements and some quick sketching, my options are either a 4 or 3 column grid. There are 8 possible combinations I can come up with for a 4 column grid, vs only 4 combinations for a 3 column grid. On the face of it, the 4 column grid should win. However, based on past experience, with a 4 column grid you can run into a slight problem on mid sized screens. The columns tend to squish too much, but at the same time, the screen is a little too wide for full-width columns. Considering this, and not wanting to spend too much time on the grid, I decide to go with a 3 column layout.

This still gives me enough variety to keep the page interesting. My next step is to figure out the column widths. At this point, I don't want to worry too much about huge screens, so I decide that I will use a `max-width` on my content area.

### Column width
Readability of body text is of great importance to me, so a good way to decide these column widths is to base them on the measure of your text. The 'measure' in typography is the line length of your body text. In *The Elements of Typographic Style*, Robert Bringhurst says that an acceptable measure for text set in a single column is 45-75 characters, including spaces. An ideal measure is 66 characters, so based on my chosen typeface, I want to get as close to this number as possible.

A confession: this part is not truly mobile-first design. This column width is going to be true for my larger screen sizes; fitting this many characters on mobile screens makes the text hard to read. Typecast has an excellent post about creating a [typographic scale for modern devices](http://typecast.com/blog/a-more-modern-scale-for-web-typography "A More Modern Scale for Web Typography"). On smaller screens, I'm going for around 35 characters per line. I am going to use their scale as a starting point for my typography, and tweak it from there.

The typeface I have chosen for my body copy is **Rooney Web Pro**. At this point, I decide to take a gamble and see what happens with my 3 column grid at a `max-width` of 1024px. I am going to use padding to create the gutters between columns, and 20px of padding on the left and right of each column looks pretty good. This gives me a `<p>` spanning 2 columns equalling 643px. Rooney Web Pro set at 20px gives me...67 characters per line on average! The text looks gorgeous at this size.