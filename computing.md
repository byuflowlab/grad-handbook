# Scientific Computing

- Guidance for setting up your mac, specific to our lab, is avilable [here](https://github.com/byuflowlab/flowlab-notebook/blob/master/tutorials/macsetup.md).  
- You should also go through our tutorial on getting setup for [LaTeX](https://github.com/byuflowlab/flowlab-notebook/blob/master/tutorials/latex.md).

## Document as You Go

- Use a lab notebook.  I recommend a digital notebook.  [Jupyter](http://jupyter.org) is one good option, but there are others.  I used hard bound notebooks for years, but now wish I hadn't.  It's really hard to find past notes, derivations, etc. once you have several notebooks. Digital copies are so much easier to search, tag, and organize.  Paper (and whiteboards) are still needed, but will be more useful to you later if you scan them, or take a picture, to archive in a digital notebook.
- **Create theory documentation (in addition to usage documentation) for any code you write**.  Any derivation you do in your notebook that is used in your code, should be transferred to an electronic format attached with the code (again, made easier if the notebook was digital to begin with).  It is very common to revisit your code later, or for someone else to want to build on it.  If the theory isn't carefully documented it's going to be very hard to remember what you did or for someone else to try to figure it out.  A few minutes now will save you hours later (both for modifying code later, and for writing the methodology in your papers).  Here are some suggested formats:
    - [Documenter.jl](https://github.com/JuliaDocs/Documenter.jl): For Julia this should be your default.  It is markdown-based and easy to use.  You can host the docs using [Github Pages](https://pages.github.com).  If on Python [MkDocs](https://www.mkdocs.org) is a good option.
    - README: if the module is very simple and only requires a short amount of documentation (e.g., a wrapper module) a README file will suffice or a README and a couple of markdown files.  (Even with other documentation options you should still always have a README to provide some a basic explanation of what the module does and how to get started).
    - LaTeX PDF: Extensive theory is probably best documented separately in LaTeX because you can cross-reference equations, references, etc.  You can then refer to it in your main documentation.
- Use Docstrings and learn what the expected format is for your programming language.
- Comment your code.  Refer to where you found equations/values (e.g., reference your documentation or a textbook/paper).
- Beginners often have one comment line per 10 lines of code, excellent programmers invert that ratio (perhaps a bit exaggerated, but good docstrings should take up a significant portion of your code).  

## Version Control and Backup

- [Version control](http://en.wikipedia.org/wiki/Revision_control) is essential.  We use version control to develop code, to write papers, to collaborate, to rollback changes, etc.  Use good commit statements so that you have a useful version history.  Version control is helpful even on individual projects.  
- Our lab uses [GitHub](https://github.com/byuflowlab) to host our repositories. If you are actively working in our research group, sign up for a GitHub account and send me your username so that I can add you to our team.  
- For stand alone codes, our repository naming convention is all lowercase.  Avoid separators where possible, but if it will help readability use a dash to separate words, not an underscore.  
- For a paper and associated code, our naming convention is leadauthorlastname[year]-shortdescription (i.e., ning2017-airfoil).
- Archive results in addition to the code that produced it. <a name="archive"></a> Also archive the code that you used to create plots.  This will save you a lot of time when regenerating plots.  Plot regeneration is often needed to create versions of your plots for your presentation, or in responding to peer-reviewer's suggestions on your publications.  
- Backup.  You **must** have your data, code, etc. backed-up in at least one other location and preferably two other locations.  At some point you will lose data if you do not have backups.  I recommend Dropbox (continuous cloud-based backup) or Box (for which we have an umlimited university subscription).

## Code Development

- Document and comment your code in detail as you go.  I said this already, but it is important and rarely done enough!
- **Unit Test!**  All major programming languages have easy to use unit test frameworks.  You need to test your code anyway so encapsulate the tests so you can run them later and help ensure correctness as you refactor later.  As you update code be sure to update your unit tests as well.
- Make effective use of whitespace and other delimiters to group logical sections together and make your code easier to read.
- Use descriptive variable names.
- If you find yourself writing a very similar piece of code more than once, you should refactor the code to create one function used in multiple places.  Having duplicate code opens up additional opportunities for bugs with version mismatches.
- Don't try to write a large program all at once.  Break it down into small pieces. For each small piece be sure to thoroughly verify and validate (V&V) it before moving on.  In this way you can build up large complex codes.
- IT 515R Scientific Computing may be helpful to you.

## Project Management

- We often use GitHub for more than just version control.  We also use it to track and discuss tasks and bugs through [Issues](https://guides.github.com/features/issues/), organize and visualize [project progress](https://www.youtube.com/watch?v=C6MGKHkNtxU), perform [code reviews](https://github.com/features/code-review), and [document](https://guides.github.com/features/wikis/).
