
# flowaround

A LaTeX package for typesetting a paragraph whose text flows around an image (or any other) box.

## Usage

In preamble:
```
\usepackage{flowaround}
```
and in the body of document:
```
\flowaround*[<number>]{<image>}[<caption>]
```
This command should come near the start of a paragraph.
Starting a paragraph with this command is also OK in most cases.

## Argument

```
{<image>}
```
Any horizontal stuffs.
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

## License

Public Domain.
