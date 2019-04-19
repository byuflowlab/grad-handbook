# Writing

## Make it a Habit
- **Write Daily.** Even if just for 15 minutes. Regular short intervals are much more productive than irregular long intervals.
- **Start writing from the beginning of your project.** Not all writing need be for the final manuscript.  Spending 10 minutes in the morning articulating the how and the why regarding the code you are going to write or the experiment you are going to conduct.  This can save you a lot of wasted time and refine your thinking.  Similarly, spending 10 minutes documenting the results after an analysis will save you lots of time later.
- **Create an environment where you can focus.**  Close your email or other things that send notifications.
- **Create accountability**.  If you have a hard time getting into the habit, record the time you spent writing and share it with someone daily.

> When performance is measured, performance improves. When performance is measured and reported, the rate of improvement accelerates.
> -- Thomas S. Monson

## Writing Tips
- **Don't spin your wheels when you start.**  I like to start by editing what I wrote the previous day (about 5 mins), then continue with new writing from there. This help me get going, and quickly gets me reoriented to writing new content.
- **Use a detailed outline.** When starting a new paper it is helpful to begin in bullet form. Slowly add, reorder, and rephrase the bullets until you have a complete outline. Get feedback on your outline.  Once you have worked out the logical flow with well-written topic sentences, filling in the details is much easier.  If you don't have clear organization early on, your paper will be much harder to fix later.
- **When writing new paragraphs just put things down on paper.** Don't try to make it perfect. This is not the time for editing, or jumping over to the web to get references. If you know you need a references, just make a note of it and keep writing.
- **Keep in mind the audience you are writing for.**
- **Use active voice.**  The use of active voice vs passive voice and first-person vs third-person has at times been a point of argument.  Traditionally, passive voice has been used in scientific publications, but today most publishers recommend use of active voice in scientific publications.
For example:
    - [Nature](http://www.nature.com/authors/author\_resources/how\_write.html): "Nature journals prefer authors to write in the active voice ("we performed the experiment...") as experience has shown that readers find concepts and results to be conveyed more clearly if written directly."
    - [Science](http://www.sciencemag.org/site/feature/contribinfo/prep/res/style.xhtml): "Use active voice when suitable, particularly when necessary for correct syntax (e.g., "To address this possibility, we constructed a Zap library . . .," not "To address this possibility, a Zap library was constructed . . . ")."
    - [A summary of over 30 books](http://eloquentscience.com/2011/02/are-first-person-pronouns-acceptable-in-scientific-writing/) on scientific writing finds that all but one advocate for active voice.
- **Be concise.**  Eliminate filler words.  Don't write like a travelogue.  Your reader is not interested in the sequence of things you did, but in a concise description of the important results.  A good exercise is take your finished draft and try to reduce its length by 10-50% (depending on how rough the draft is).
- **Clearly define the problem and your solution in the introduction.**  Don't make your reader read between the lines.  Early on you must clearly answer these questions:
    - What is the problem?
    - Why is it important?  
    - What has been done already?
    - What is your approach and how does is uniquely and effectively address the problem?  
- **Be specific.**  Avoid vague phrases like "the CFD results mostly agree with the experimental data" instead say "the CFD results match the experimental data to within 2% across all stations"

## Editing
- **Get feedback early** from people both inside and outside of your field. Before submitting a paper to your advisor of supervisor make sure at least two of your peers have reviewed it.
- **When you receive feedback, just listen**. Don't try to explain what you meant, just listen. If they didn't understand it, then it wasn't clear.
- **Take advantage of university writing resources** like the BYU's Writing Center.
- **Read your text out loud to yourself.**
- **A writing group can be very effective.**  For example, meet once a week in a group of size 3-4.  Each of you share an excerpt you wrote that week (one page max), and everyone else provides feedback (10 minutes).  Rotate through each person.


## Tools

- **Use [LaTeX](https://en.wikipedia.org/wiki/LaTeX)**.  LaTeX is a typesetting program widely used in STEM fields.  It produces nicely typeset documents while allowing you to focus on the content.  There is a learning curve, but it's well worth it.  LaTeX really shines with formatting mathematical content, making it easy to cross-reference figures/tables/equations/citations, and allowing quick document-wide style changes (i.e., for a different journal).  Additionally, it is a plain text format meaning that version control is easy and effective. Some people can work wonders with programs like Microsoft Word, and if that works for you that's great&mdash;except if you are a student in my lab, then you must use LaTeX :)

- **[Overleaf](https://www.overleaf.com) is particularly useful for beginning LaTeX users**.  It's like Google Docs for LaTeX.  It allows you to edit your documents on the web without installing anything, and allows you to do so collaboratively.  Personally, I prefer a dedicated text editor so I can define my own macros, but overleaf has some nice features that make tracking changes and diff'ing easier.

- **Use version control for your paper and tag important milestones.** Every paper should correspond to a repo in our Github organization.  Use this naming convention lastnameYear-short-description.  Your repo should contain not just the latex and figures files, but all the code that is used to generate the data and figures.  Sometimes you will use an external code (or another code that we maintain separately in our organization).  In julia your manifest will be able to track all the package versions, if using Python you need to do this manually (e.g., with a text file that notes the version (or commit ID) of the code(s) you used).  Use an appropriate .gitignore file (see [here](https://gist.github.com/kogakure/149016) for a good start) so that you only commit the source files and not intermediate build files. The one exception is that I recommend committing the pdf for submitted versions (conference submission, journal preprint, journal final version).  These won't change so they won't cause your git repo to blow up in size, but having them easily accessible will be quite convenient. Provide clear comments or tags on the important milestones (e.g., initial submission to journal) so that it will be easy to compare changes later. You will need to detail changes in your response to reviewer comments.  

- **Use [latexdiff](https://www.ctan.org/tex-archive/support/latexdiff?lang=en) when sending a revised version of your paper**.  latexdiff is a diff for latex files (shows changes between two versions).  If your advisor or other reader sends you suggested edits, it can be helpful to send a diff'ed version back in addition to the full text so that the reviewer can more quickly focus on what has changed.  This is also useful when submitting a revision during the journal review process.  If you completely overhaul your paper then a diff isn't going to be very helpful.

- **Use a BibTeX manager (on a Mac I recommend [BibDesk](http://bibdesk.sourceforge.net)**).  BibTeX is the standard bibliography format used for LaTeX documents.  You can of course just use a regular text editor, but using a manager helps to make sure your key-values are formed correctly, preview results, apply changes across multiple entires, etc.  I keep all of my BibTeX data in one file, rather than create separate files for each paper (unless working with a one-off collaborator).  There are other good paper management systems like Mendeley, and Papers, but their BibTeX support has always been subpar and so I can't recommend them.  BibDesk is great because the file format is BibTeX.

- **Use a tool that facilitates automatic importing of references**.  Various tools exist, but if you are on a Mac, and own the paid version of [Alfred](https://www.alfredapp.com), then you might be interested in the [Reference Importer Workflow](https://github.com/andrewning/alfred-workflows-scientific#reference-importer) I developed or the free (but somewhat simplified) app I made [here](https://github.com/byuflowlab/bibteximport).  This app will search references using any citation metadata (e.g., title, author, etc.), import the BibTeX into BibDesk (or copy it to clipboard for other applications), and if possible download and link the PDF as well.  It uses crossref to find articles, and Google Books for books.



## Figures

- **Use vector-based graphics whenever possible (e.g., pdf, eps), if not possible, for example with a CFD screenshot, then make sure the bitmap is sufficiently high resolution.**  High-quality figures are crucial to a good paper. Bitmap images are made up of pixels.  That means that if you zoom in enough they will look pixelated.  Vector images, by contrast, are mathematically defined so that you can keep zooming in and the image will always look perfectly sharp.  This is important when viewing graphics on electronic devices as readers will often want to zoom in on an image.  Many of your graphics will be generated through a programming language and those are already mathematically defined so it would be a real shame to save it as a bitmap.  
- **Figure captions should use full sentences, and be descriptive.**  A reader should be able to understand your figure just from the figure and its caption, without having to search through the text.
- **Don't use rainbow colormaps for contour plots.**  The ordering of the rainbow colormap is nonintuitive and does not vary continuously in luminance. The result is an obscuring of details and the perception of artificial boundaries between hues.  This is especially problematic because the default for many contour plots is the rainbow colormap.  Recently, both [Matlab](http://blogs.mathworks.com/steve/2014/10/20/a-new-colormap-for-matlab-part-2-troubles-with-rainbows/) and [matplotlib](http://matplotlib.org/users/colormaps.html) have changed the default to a colormap that is more perceptually uniform.
- **Don't accept the defaults of your plotting program, rarely are they well suited for publication-quality plots**.  It's worth creating some nice defaults and saving them in your .matplotlibrc file (or in Export Setup for Matlab).  Usually I try to optimize my figures to a 3 inch width, which is a typical column size in a scientific journal.  Make sure to set the font size is large enough so that all labels are readable.
- **Save the script and the data you used to generate your figures**.  You *will* need to regenerate them again later, either for revisions, or for a presentation in which you may want different fonts/colors. Taking a few minutes to do this now will save your hours later.
- **Each figure should have a clear message---remove anything extraneous**.  Favor direct labels over legends when possible.  Don't put in background grids unless there is a clear justification.  Often, the top and right border lines just add unnecessary clutter.
- **Save figures with a transparent background in case you or I need to reuse them in a presentation later**.  In matplotlib you just add `transparent=true` or even better, put `savefig.transparent : True` in your matplotlibrc file so you don't have to remember.


## LaTeX Logistics
- If you use a period that doesn't end a sentence, you must use a tilde or the spacing will be wrong.  For example, Dr.~Bob.
- Besides the obvious packages here are a few others I recommend:
    - hyperref with the colorlinks and allcolors option set&mdash;this will add hyperlinks to your citations, figures, etc. making it easier to read
    - amsmath&mdash;provides a whole bunch of useful math environments and commands
    - cite&mdash;groups sequential citations together ([1,2,3,4,7,8] becomes [1-4,7-8])
    - subfig&mdash;create subfigures
    - booktabs&mdash;nicely formatted tables
    - cleveref&mdash;consistently format cross referencing styles Figure, Fig., fig., etc., and change them all easily
- Quote properly: ````quote''`` not ``"quote"`` (opening backticks and closing single quotes), and use hyphens and dashes properly: - hyphen, -- n-dash, --- m-dash.  
- Actual words or units in equations should be typeset with \text (i.e., $V = 30 \text{m/s}$).
- If using an inline equation, rather than a displayed equation, use "/" instead of "\frac".
