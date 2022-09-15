This is like google docs or microsoft word. However, you edit a code file which then produces a ready to publish document.

Every document has a .tex file

A document starts with a pre amble which is roughly the settings of your text, \document class is always included. Special syntax is added with the environment variable. If you want your text to be in a special environment your write:

begin{environment}

...

end{-.-}

You can structure your text with sections and laTeX will automatically connect to \tableofcontents command.

You can make a list with the environment "itemize"

You can make a table with the environment tabular, you can decide how it will look by providing arguments about the columns when you initialize the table. You can make lines between row with \hline - horizontal line. - [[Tabular example]] 

A very nice package is [[bibtex]].