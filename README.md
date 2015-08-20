# Overview
The goal of this project is to translate the freely-licensed materials created by the [African Storybook Project](http://africanstorybook.org) into all of the world's languages so that children everywhere can enjoy these wonderful African stories and create new ones in the same spirit.

All languages are welcome, although translations into African languages should usually be directed to the African Storybook Project main site. We are particularly interested in translations into languages that have very few resources for early childhood learning. For example, if you are involved in indigenous language revitalization, we would love it if you could join the project.

# Structure
Each top level folder represents a language, identified by its [ISO 639-1](http://en.wikipedia.org/wiki/ISO_639-1) or [ISO 639-3](http://en.wikipedia.org/wiki/ISO_639-3) code, with a preference for the ISO 639-1 "Alpha-2 code", if it exists. For major languages, this code is usually two characters long (e.g., `es`, `zh`, `ar`), but some languages may have three characters (e.g., `yue`).

Within each folder, files are grouped by name. The base filename for each story consists of the _story number_ (a four-digit index number that unambiguously identifies the story within the collection) followed by an underscore, and then the translated name of the story in lower case with any spaces replaced by dashes. For example, the Norwegian story _En veldig høy mann_ is story `#0001`, so the base filename is `0001_en-veldig-høy-mann`, and associated files include `0001_en-veldig-høy-mann.txt`, `0001_en-veldig-høy-mann.pdf`, `0001_en-veldig-høy-mann.ogg` etc.

A list of stories by index number can be found [here](https://github.com/global-asp/global-asp/tree/master/INDEX.md). The list includes links back to the original versions of each story on the African Storybook Project. Stories are assigned an index number in the order that they are translated; if you are translating a new story for the project just add it to the end of the list and assign it a new index number in sequence.

# File formats
The availability of stories in multiple formats is beneficial for others who might wish to use, adapt, or translate them into other languages. At a minimum, each story should include the following formats:

File format | Extension | Notes
------------|-----------|------
Text | .txt | A plain text file containing the full text of the story as well as author and license information
OpenDocument Graphics | .odg | A LibreOffice Draw document containing the full story text and illustrations
PDF | .pdf | A PDF version of the story exported from LibreOffice Draw

Optional extra formats can include:

File format | Extension | Notes
------------|-----------|------
Ogg Vorbis | .ogg | An Ogg Vorbis audio file of the story being read aloud
MP3 | .mp3 | An MP3 audio file of the story being read aloud
EPUB | .epub | An electronic book format version of the story
Zipped HTML | .html.zip | A compressed folder containing an HTML version of the story and any associated illustrations (preferably saved as PNG files)

Videos should be uploaded to a video hosting site and linked in the `story_name.txt` file.

# Contributing
All contributions welcome! Here are some ideas for ways to get involved:

- Start a new language subfolder for a language we don't have yet
- Record audio/video for stories that have any
- Proofread / correct errors in existing stories
- Create a new translation of a story from the [African Storybook Project site](http://africanstorybook.org/)
- Create a new adaptation/remix of a story in the project

# License
This project is released under the same license as the African Storybook Project. In other words, except where otherwise noted, all content is licensed under the Creative Commons Attribution 4.0 Licence.
