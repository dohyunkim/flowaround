
# flowaround

A LaTeX package for typesetting a paragraph (or more) whose text flows around an image (or any other) box.

## Usage

In the preamble:
```
\usepackage{flowaround}
```
and in the body of document:
```
\flowaround*[<number>]{<image>}[<caption>]
```
This command should come near the start of a paragraph (on the fist line of a paragraph).
Starting a paragraph with this command is OK in most cases.

## Argument

```
{<image>}
```
Any horizontal stuff.
When inserting an image, use `\includegraphics` command for yourself.

## Options

```
*
```
puts the image box at the right side of a paragraph.

```
[<number>]
```
moves the image box downwards by `<number>` lines.

```
[<caption>]
```
typesets `<caption>` below the image box.
For real LaTeX captions, use `\captionof` command from caption package.

```
\def\flowaroundhmargin{1em}
```
sets the horizontal margin beside the image box, default value being `1em`.

```
\def\flowaroundvmargin{1ex}
```
sets the vertical margin below the image box (including the caption, if any),
default value being `1ex`.

```
\def\flowaroundraisebox{0pt}
```
raises the image box (including the caption, if any) by the amount specified,
default value being `0pt`.

## License

Public Domain.
