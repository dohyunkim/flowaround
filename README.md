
# flowaround

A LaTeX package for typesetting a paragraph (or more) whose text flows around an image (or any other) box.

## Usage

In the preamble:
```latex
\usepackage{flowaround}
```
and in the body of document:
```latex
\flowaround*[<number>]{<image>}[<caption>]
```
This command should come near the start of a paragraph (on the first line of a paragraph).
Starting a paragraph with this command is OK in most cases.

```latex
\suppressflowaround
```
suppresses the flowaround effect for the scope.
It could be useful at the start of a footnote text while flowaround is active in the main text.

## Argument

```latex
{<image>}
```
Any horizontal stuff.
When inserting an image, use `\includegraphics` command for yourself.

## Options

```latex
*
```
puts the image box at the right side of a paragraph.

```latex
[<number>]
```
moves the image box downwards by `<number>` lines.

```latex
[<caption>]
```
typesets `<caption>` below the image box.
For real LaTeX captions, use `\captionof` command from caption package.

```latex
\def\flowaroundhmargin{1em}
```
sets the horizontal margin beside the image box, default value being `1em`.

```latex
\def\flowaroundvmargin{1ex}
```
sets the vertical margin below the image box (including the caption, if any),
default value being `1ex`.

```latex
\def\flowaroundraisebox{0pt}
```
raises the image box (including the caption, if any) by the amount specified,
default value being `0pt`.

## License

Public Domain.
