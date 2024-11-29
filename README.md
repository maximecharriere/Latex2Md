# Latex2Md URL Generator

Generate LaTeX equations with the official GitHub renderer.

## How to use it

Github doesn't render LaTeX equations in markdown. So equations in .md files or comments in issue, pull request and gist will not be displayed as you would like.  
However, GitHub support the equations in Jupyter Notebooks preview. See [Jupyter Notebooks Examples](https://github.com/maximecharriere/Latex2Md/blob/main/equations.ipynb).  

Looking for how GitHub renders equations in Jupyter Notebooks, we see that the following link is called:  
`https://render.githubusercontent.com/render/math?math=<LATEX EQUATION>`

This link return a .svg image, so we can use it as an image source in our Github Markdown.  
However, some characters in the equation cannot be written directly in the URL. New browsers interpret most characters correctly, but some characters like the "+" must still be replaced by their HTML code.
**The URL generator on this website automaticaly replaces all characters not correctly interpreted by new and old browsers**. The URL will be longer and less understandable, but more compatible.

It is recommended to use the HTML syntax because it is more compatible, produces fewer errors and takes into account the background color.

## Credit

[A hack for showing LaTeX formulas in GitHub markdown.md](https://gist.github.com/a-rodin/fef3f543412d6e1ec5b6cf55bf197d7b) gist by a-rodin.
