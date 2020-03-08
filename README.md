# Global ASP - African Storybook Project Stories for the World

## Overview

The goal of this project is to translate the freely-licensed materials created by the [African Storybook Project](http://africanstorybook.org) into all of the world's languages so that children and language learners everywhere can enjoy these wonderful African stories and create new ones in the same spirit.

All languages are welcome, although translations into African languages should usually be directed to the African Storybook Project main site rather than here. We are particularly interested in translations into languages that have very few resources for early childhood learning. For example, if you are involved in indigenous language revitalization, minority language education, or heritage language learning, we would love it if you could join the project.

## PDFs

All of the audio, images, and PDFs associated with this project can be downloaded from the links found [here](https://storybookscanada.ca/downloads/).

## Structure

Each top level folder represents a language, identified by its [ISO 639-1](http://en.wikipedia.org/wiki/ISO_639-1) or [ISO 639-3](http://en.wikipedia.org/wiki/ISO_639-3) code, with a preference for the ISO 639-1 "Alpha-2 code", if it exists. For major languages, this code is usually two characters long (e.g., `es`, `zh`, `ar`), although some languages may have three characters (e.g., `yue`).

Within each folder, files are grouped by _story number_ (a four-digit index number that unambiguously identifies the story within the collection). The _basename_ for each story consists of the _story number_ followed by an underscore (`_`), and then the translated name of the story in lower case with any spaces replaced by dashes (`-`).

All of the source files in the repository are stored in Markdown format, and consist of the _basename_ plus the Markdown extension `.md`. Alternate, binary and other formats generated from the source files are named with the _basename_ followed by the appropriate format extenstion.

For example, the Norwegian story _En veldig høy mann_ is story `#0001`, so the base filename is `0001_en-veldig-høy-mann`. The file containing the story source is `0001_en-veldig-høy-mann.md`, and other formats included in the download package include `0001_en-veldig-høy-mann.txt`, `0001_en-veldig-høy-mann.pdf`, `0001_en-veldig-høy-mann.epub` etc.

A list of "core" translateable stories by index number can be found [here](https://github.com/global-asp/global-asp/tree/master/INDEX.md). The list includes links back to the original versions of each story on the African Storybook Project.

Due to an absence of an unambiguous id for each story on the ASP site, stories have been assigned an index number randomly and/or in the order that they are translated. If you are translating a new story for the project just add it to the end of the list and assign it a new index number in sequential order.


## File formats

The availability of stories in multiple formats is beneficial for others who might wish to use, adapt, or translate them into other languages. At a minimum, we aim to provide stories in the following formats:

File format | Extension | Notes
------------|-----------|------
__Markdown__ | .md | The source format: all translations are stored in this format, from which the other formats are automatically generated
EPUB | .epub | An electronic book format version of the story, suitable for use with e-readers
HTML | .html | An HTML file containing the text of the story, with images linked to an included `img` folder (see JPG format above)
HTML slideshow | _slides.html | A standalone html slideshow in [DZSlides](http://paulrouget.com/dzslides/) format
JPG | .jpg | Extracted images for each story in a separate `img` folder; these are refered to by the HTML and slideshow files, and are used to compile other formats such as PDF and Epub
PDF | .pdf | A PDF version of the story compiled from the Markdown source text and image bank
Text | .txt | A plain text file containing the full text of the story as well as author and license information; the content of this file is very similar to the .md source, but may be easier to read/open/edit on some systems or for users not used to working with Markdown

The following multimedia formats are now available as part of the [gasp-audio](https://github.com/global-asp/gasp-audio) project:

File format | Extension | Notes
------------|-----------|------
Ogg Vorbis | .ogg | An Ogg Vorbis audio file of the story being read aloud
MP3 | .mp3 | An MP3 audio file of the story being read aloud

Audio files are automatically cut into individual sections and turned into [audio slideshows](https://global-asp.github.io/audio/). Please see the [gasp-audio](https://github.com/global-asp/gasp-audio) project for details.

## Source format

The source files in this repository are stored in [Markdown format](https://help.github.com/articles/markdown-basics/). You can download pre-formatted (untranslated) Markdown files from the [ASP Source](https://github.com/global-asp/asp-source) project that have been extracted from the original ASP pdfs and automatically converted, for all of the core stories in the master index.

There are a few conventions that are used in addition to basic Markdown formatting to allow the files to be easily converted to other formats.

### Story title

The title of the story is indicated at the top (first line) of the Markdown file, generally following a hash character and a space (`# `). The title should be on a single line (no linebreaks). If there is a sub-title or other information about the story that should be on the front page (aside from the author name -- see the [Metadata section](#metadata) below), it can be included on the following lines (__not__ preceded by `#`).

### Page breaks

Page breaks within the story are indicated by two `##` characters on a separate line, followed by the text of the following page.

### Sections

For the purposes of this project, stories are conceived of as individual pages consisting of a single image and accompanying text, with surrounding front and back covers and associated metadata. Almost all of the ASP stories conform to this format, and it has been followed here as well, which makes generation of other formats much easier.

Sections are defined as the content found between page break markers (`##`), or between a page break marker and the beginning/end of the file.

The first section is roughly equivalent to the cover page and should only contain the title of the story and (in rare cases) a sub-title or other explanatory text that should go underneath the title on the cover. Metadata such as the author name and language of the story will be automatically included when storybooks are generated and should __not__ be in the first section.

The last section is equivalent to the final page or back cover of the storybook, and contains relevant [metadata](#metadata) about the story. See the [Metadata section](#metadata) below for details about what to include here.

### Images

Images from the [ASP Image Bank](https://github.com/global-asp/asp-imagebank) are automatically included in the generated binary formats and are __not__ indicated in the markup. There is no need to create image links or link to image urls or filenames within the Markdown source.

### Metadata

Story metadata is included in the [last section](#sections) of the Markdown source file.

The metadata section should include the following information:
* License
* Writer
* Illustrator
* Translator
* Language

These should each be on a separate line, and each item of metadata should not be more than a single line. There is some flexibility with the wording, but ideally the names should be as consistent as possible. Any additional fields or information will be removed from the generated storybooks.

A typical metadata section should look something like this:

    * License: [CC-BY]
    * Text: Clare Verbeek
    * Illustration: Mlungisi Dlamini
    * Translation: dohliam
    * Language: zh

Notes:
* The License information is included between square brackets (`[]`) and should be one of either `[CC-BY]` or `[CC-BY-NC]` in accordance with the original story license
* The Translator field should indicate your name rather than the name of the person who translated the original ASP story (if the original is a translated or versioned story)
* The Language field should exclusively use the appropriate language code for the language you are translating __into__

## Download

**NOTE**: These are now out of date. For more current downloads (PDF and audio in a variety of formats), see [this link](https://storybookscanada.ca/downloads/). A build toolchain for compiling your own binary formats from the raw Markdown files will be added here soon. See also [Nairobi CSS](https://github.com/global-asp/nairobi-css) for a quick way to use the Markdown files in this repository directly in a custom built online site.

***

Pre-compiled binary releases containing Markdown source files along with alternate formats (specifically __PDF__, __ODT__, __epub__, __HTML__, __HTML slideshow__, __jpg__, and __plain text__) are available on the [releases page](https://github.com/global-asp/global-asp/releases).

See the download lists (files named `README.md`) in the individual language folders for download links for specific languages.

## Contributing

All contributions are welcome! (This includes reporting issues.)

If you are interested in translating any of the stories, [__start here!__](https://globalstorybooks.net/translator/) This link will take you to the [Global Storybooks Translator app](https://globalstorybooks.net/translator/), which makes translating stories quick and easy. The app starts with the shortest and simplest stories first, and lets you gradually work up to translating more complicated stories as you progress -- though you can skip forwards or backwards and translate any story you like at any time.

You are also more than welcome to submit a pull request directly to this repo with your translation / correction. You should use the .md files in this repo (which are also included in the [binary releases](#download)), and follow the [existing format](#source-format). This is the only format accepted for pull requests to this Github repository.

See the [Source format section](#source-format) above for information about getting pre-translated Markdown files for all the ASP stories.

If you're already comfortable with Github and version control, here are some other ideas for ways to get involved:

- Start a new language subfolder for a language we don't have yet
- Proofread / correct errors in existing stories
- Create a [new translation of a story](https://global-asp.github.io/translator/)
- Record audio/video for stories that don't have any (we are actively looking at ways to manage audio and video formats, but for now the best place to put them is probably YouTube or a similar site)
- Create a new adaptation/remix of a story in the project (these can be linked to in the wiki)

You can also send .md or plain text files to globalafricanstorybook@gmail.com with your translation or correction and they will be included in the project with attribution.

## License

This project is released under the same license as the African Storybook Project. In other words, except where otherwise noted, all content is licensed under the [Creative Commons Attribution 4.0 Licence](https://creativecommons.org/licenses/by/4.0/).

All of the ASP and Global-ASP stories are [Creative Commons-licensed](http://creativecommons.org/). By contributing a translation to the project you agree to release your work under a Creative Commons license (either [CC-BY](https://creativecommons.org/licenses/by/4.0/) or [CC-BY-NC](https://creativecommons.org/licenses/by-nc/4.0/)) in accordance with the license of the original story.

Many thanks to the original authors and illustrators, our translators, and the many people who have volunteered to check and proofread the translations.
