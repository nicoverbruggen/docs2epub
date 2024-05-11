# docs2epub

Prerequisites:

- You must have `pandoc` installed
- You must have some source files in the `src` directory

For example, you can use this to generate an epub file for all of the Laravel docs. Just put the Markdown files in the `src` directory, and run the following command:

	pandoc src/*.md -o Docs.epub -c ./epub.css --metadata title="Docs"

Your book will then be available as `Docs.epub`. You can also set some additional metadata.