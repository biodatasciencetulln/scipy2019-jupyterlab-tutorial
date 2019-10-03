# Exercises 1

Attempt the following. These are _guidelines_, feel free to err on the side of workflow and
options that suits _you_ if you find them best.

## View this file as rendered markdown.

Right-click on the `Exercise1.md` file to open it as rendered markdown called "Markdown Preview".

## Layout

Create a new notebook.

Arrange the notebook and rendered markdown side-by-side. Then arrange them, one on top and one on bottom. Then arrange them in a single panel with two tabs. Then split them out again to side-by-side.

## Notebook operations

- Open the Jupyter context menu (right-click) and compare it to the regular browser context menu (Shift+right-click). Note that this works in the notebook and in the terminal!

- Change the first cell to markdown, and write some markdown with
    - Bold
    - Italic
    - Code (triple backtick fences ` ``` `, or indented 4 spaces)
    - The Markdown parser in the Jupyter Notebook is [MathJax](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)-aware, and you can use mathematical expressions using the MathJax subset of Tex and LaTeX. Note that this is not regular Markdown, but a feature of Jupyter notebooks. Try (inline and formulas): `$f(x) =  a.x^2+b.x+c$`, `$$x_\pm = \frac{-b \pm \sqrt(b^2-4ac)}{2a}$$`
    - Reference: https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Working%20With%20Markdown%20Cells.html

- Create a code cell and evaluate it, printing "Hello SciPy"
    - Experiment with the run shortcuts `Ctrl-Enter`, `Shift-Enter`, and `Alt-Enter` and note the differences between them (see the Run menu for help).
    - Try importing `pandas`
    - Evaluate `pandas?` to get the help on the pandas library.
    - Use tab completion: `pandas.D<tab>` to get tab completion on the pandas library. Note that completions can take a few seconds the first time while the library gets inspected.
      - If tab completion is slow/buggy, execute `%config Completer.use_jedi = False` to use a less sophisticated completion mechanism
    - Complete to `pandas.DataFrame(`; place the cursor after the open bracket and press `Shift-Tab` to get quick help.
    - Get help:
        - Regular way: `help(pandas)`
        - Ipython way: `pandas?`
        - Ipython way to access the source code: `pandas.DataFrame??`
          - Use the context menu to enable scrolling
    - To always see the info about the current function, use the "Contextual Help" (via right-click, keyboard shortcut or new Launcher).
        - Move the contextual help tab somewhere so that you can see both it and the notebook.
        - Type `pandas.read_csv(` to see the interactive function help.

- Open/process csv/tsv files
    - Open `'../data/iris.csv'` as a standalone CSV file
    - Use panda’s `read_csv` to load `'../data/iris.csv'` into a dataframe, display this dataframe
    - Use `%matpltolib inline` to allow inline graphs
    - Make a scatter plot of `sepal_length` vs `sepal_width`


# More advanced notebooks

- Move a cell by dragging (within a notebook or between notebooks)
- Use the View menu, or click the blue bar, to collapse and expand an input and an output.
- Use the context menu to enable scrolling in a cell that has lots of output.
- Try “Create new view for output” in the context menu of an output. Modify and execute the cell again to see the mirrored output update (will learn more in section 2)
- Learn the various keyboard shortcuts through the menu and the command palette.
