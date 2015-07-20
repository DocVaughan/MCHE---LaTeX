# Useful LaTeX Snippets

## Unbalanced brackets
	M = \left\{ \begin{array}{ll} 2 + 2 & \mbox{if } t < 1 \\    
		1 + 3 & \mbox{if }  t > 2 \end{array}\right.
		


## List Spacing
	\usepackage{enumitem}

	\begin{itemize}[noitemsep,nolistsep]
		\item Item 1	
		\item Item 2
		\item \ldots
	\end{itemize}


## If/then
http://tex.stackexchange.com/questions/5894/latex-conditional-expression

	\newif\ifpaper
	
Then either

	\papertrue % or
	\paperfalse

And to use it:

	\ifpaper
	  % using paper
	\else
	  % electronic
	\fi

	
## Resetting the page counter

	% reset the page counter, so it begins with the page of the introduction section
	\setcounter{page}{1} 
	
	
## Draft Watermark

	\usepackage{draftwatermark}
	% \SetWatermarkText{Watermark Text} % Will default to DRAFT
	\SetWatermarkScale{5}