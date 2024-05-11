# docs2epub

Prerequisites:

- You must have `pandoc` installed
- You must have some source files in the `src` directory

For example, you can use this to generate an epub file for all of the Laravel docs. Just put the Markdown files in the `src` directory, and run the following command:

	pandoc src/*.md \
		--from gfm \
		-c ./epub.css \
		-o Docs.epub \
		--epub-embed-font="./fonts/*" \
		--metadata title="Docs"

Your book will then be available as `Docs.epub`. You can also set some additional metadata.

## License

This README and additional files are released into the public domain.

However, please note that the fonts included in the `fonts` directory are available under their original licenses, which should allow them to be embedded into epubs.