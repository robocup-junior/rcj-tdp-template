# RoboCupJunior Technical Description Paper (TDP) Starter Template

Use this template to describe your team's project and learn LaTeX. It is
intended for teams across RoboCupJunior. The repository contains the
paper source, example images and the Springer document class. The sample paper
describes a fictional Rescue Line robot and fictional test results. Whether
your team takes on a Rescue challenge, plays Soccer or performs in OnStage, use
the prompts to tell the story of your own project.

The template uses the same LNCS document class used for the [2026 RoboCup
Symposium](https://2026.robocup.org/symposium/). It is adapted for Junior teams
and is not an official Symposium or Junior template.

**Check your event's rules before you submit.** Your event may require a
particular form, template or poster. Use this paper to prepare your work, then
transfer it to the required format. It does not replace separate submissions
such as a bill of materials, video or code.

## Start with Overleaf

[Open the read-only template in Overleaf](https://www.overleaf.com/project/6af6f47cfb32ee29ccefb13d/share#469599663820a00520a03a7ce97997903d96aa99559aee36).
You can view the source and preview without signing in. To edit your own copy:

1. Sign in to Overleaf or create an account
2. Open the link above and select **File → Make a copy**
3. Name the copy and select **Copy**. The new project belongs to your account
4. Open `main.tex`, read the comments starting with `%`, and replace the
   placeholders and examples with your team's work
5. Select **Recompile** to update the preview, then **Download PDF** when ready

To add pictures, follow the instructions under "Upload the ZIP to Overleaf."

The Overleaf project is a snapshot of this template. Repository changes do not
automatically update it. The download instructions below are an alternative if
you want to use the repository files directly.

## Download the template

On the repository page on GitHub, click the green **Code** button and select
**Download ZIP**. Save the ZIP file on your computer. If you have Git installed,
you can also clone the repository using its URL from the **Code** menu.

The ZIP contains `main.tex`, `llncs.cls` and the images in `figures/`.
Keep these files together. You will edit `main.tex`. The `llncs.cls` file
controls the layout, and the images appear in the example figures.

## Upload the ZIP to Overleaf

1. Open [Overleaf](https://www.overleaf.com/) and sign in or create an account
2. Select **New Project → Upload Project**, choose the downloaded ZIP and
   upload it
3. Open `main.tex` in the file list and click **Recompile** to see the PDF
4. Write your team's work below the comments in each section, replacing the
   examples. Comments begin with `%` and do not appear in the PDF
5. Recompile as you work, then select **Download PDF** to save your paper

To add a picture, upload a PNG, JPG or PDF file to the `figures` folder. In
`main.tex`, change the path inside the existing `\includegraphics` command.
For a file named `robot.png` in `figures`, use
`\includegraphics{figures/robot.png}`. The comments next to the example
explain the figure and its caption.

## Write on your computer

Extract the ZIP and open the resulting folder. Install a LaTeX distribution,
such as [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/).
A LaTeX editor can help, but a plain text editor works too.

Open `main.tex` in your editor and replace the placeholders and examples.
To build the PDF, open a terminal in the extracted folder and run:

```sh
pdflatex main.tex
pdflatex main.tex
```

Run the command twice to update figure, table and citation numbers, then open
`main.pdf` in the same folder. Repeat these commands after editing the paper.
The included `llncs.cls` provides the document class. A standard LaTeX
installation provides the compiler and standard packages.

If the build fails, read the first error in the terminal or `main.log` and
check the line it mentions. A missing `}` or an unescaped `%` is a common
cause. If an image is missing, check its filename, capitalization and folder.

## Make the paper yours

- Read the comments in `main.tex` for writing prompts. Choose the questions
  that fit your league and project
- Keep, rename or remove sections as appropriate for your work and event
- Replace or remove the example figures, table, equation, list and citation
- Credit designs, code, libraries and other sources you used. Explain what
  your team made or adapted and follow your event's rules on assistance and AI
- Use names, photographs and contact details only as your event and team permit
- Before submission, check for remaining placeholders and examples. Check
  your event's page limit, format and separate submission requirements

## LaTeX basics

- `\section{Title}` starts a section. Write text below it
- Leave a blank line between paragraphs
- `%` starts a comment. Write `\%` to show a percent sign. Write `\&`, `\_`,
  `\#` and `\$` for the corresponding characters in ordinary text
- Use `\textbf{important text}` for bold and `\emph{a term}` for emphasis
- `\ref{fig:system}` refers to the figure with `\label{fig:system}`
- `\cite{rcj}` refers to the source with `\bibitem{rcj}` at the end of the file
- See the comments in `main.tex` for the image, table, equation, list and
  reference examples

See [THIRD-PARTY.md](THIRD-PARTY.md) for the included document class's license
and attribution.
