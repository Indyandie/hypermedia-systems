# EPUB

## Dependencies

- [asciidoctor](https://docs.asciidoctor.org/)
- [pandoc](https://pandoc.org/)
- [fd](https://github.com/sharkdp/fd)
- [sd](https://github.com/chmln/sd)

## Assembly Line

> [!warning]
>
> This is very convoluted...

1. Copy books and escape some characters
1. Convert `adoc` files to `xml` with asciidoctor
1. Rename name some files to keep the chapter order
1. Convert `xml` files to `md` with pandoc
1. Adjust headings and add chapter titles
1. Copy images and adjust `svg` fill and background
1. Covert `md` to `epub`

## Generate EPUB

Under the `epub` directory run `./epub-script`
