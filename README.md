# Academic_CV

A LaTeX template for academic CV, available for English and Simplified Chinese.

## Compiler and Environment

- Must be compiled with **LuaLaTeX**;
- Developed with [MikTeX](https://miktex.org/) on Windows, should be equally fit for [TeXstudio](https://www.texstudio.org/) and [Overleaf](https://www.overleaf.com/) on other OSs.

## Fonts

All fonts required by this template are freely available.
They are saved in `fonts` folder in static `.ttf` or `.otf` formats to keep the style consistent.

Latin alphabet, punctuation & numbers:

- Serif (text): [Cardo](https://fonts.google.com/specimen/Cardo), including regular, bold, and italic fonts; bold-italic (small capitals) is not available, which leads to the italic (regular) font.
- Sans serif (title): [Lato](https://fonts.google.com/specimen/Lato), including regular, bold, and italic fonts; bold-italic (small capitals) is not available, which leads to the italic (regular) font.

Chinese characters & punctuation:

- Serif (text): [Source Han Serif (思源宋体)](https://fonts.adobe.com/fonts/source-han-serif-simplified-chinese), including regular and bold fonts; italic, bold-italic, and small capitals are not available, which leads to the regular font.
- Sans serif (title): [Source Han Sans (思源黑体)](https://fonts.adobe.com/fonts/source-han-sans-simplified-chinese), including regular and bold fonts; italic, bold-italic, and small capitals are not available, which leads to the regular font.

Hyperlinks are colored in blue RGB: (0,0,199).
This setup can be overwritten with `\definecolor` and `\hypersetup` in tex preamble.

## Usage

For English CVs, call `\usepackage{academicCV_en}`; for Chinese CVs, call `\usepackage{academicCV_zh}`.
The defined commands are listed below with necessary explanations.

| Command                           | Comment     |
| :-------------------------------- | :---------- |
| `\myname{<name>}`                 | Mandatory   |
| `\myaddress{<address>}`           | Mandatory   |
| `\myposition{<position>}`         | Mandatory   |
| `\mytel{<phonon>}`                | Mandatory   |
| `\myemail{<email>}`               | Mandatory   |
| `\mysite{<website>}`              | without 'https://' |
| `\makeheader`                     |             |
| `acmedia` environment             | Academic social media |
| `\EntrySeparator`                 | Add a pipe '\|' between items |
| `\myGoogleScholar{<url>}{<text>}` | As `\href`  |
| `\myORCID{<url>}{<text>}`         | As `\href`  |
| `\myResearchGate{<url>}{<text>}`  | As `\href`  |
| `\myAcademia{<url>}{<text>}`      | As `\href`  |
| `\myGitHub{<url>}{<text>}`        | As `\href`  |
| `\myLinkedIn{<url>}{<text>}`      | As `\href`  |
| `\myTwitter{<url>}{<text>}`       | As `\href`  |
| `\experience{<position>}{<date>}{<organization>}{<location>}{<description(optional)>}` | An entry of education / employment experience |
| `\award{<name>}{<date>}{<event>}{<description(optional)>}` | An entry of fellowship / honor / award etc. |
| `\grant{<name>}{<date>}{<source>}{<amount(optional)>}{<description(optional)>}` | An entry of research grant |
| `paperlist` environment, with option `ascending=<true/false>` | List of papers, numbered in ascending / descending order |
| `\journal{<author>}{<title>}{<journal>}{<year>}{<volume(optional)>}{<issue(optional)>}{<page(optional)>}{<DOI(optional, without https://doi.org/)>}{<other comments(optional)>}` | Journal paper entry in `paperlist` environment |
| `\preprint{<author>}{<title>}{<journal/server>}{<status>}{<year>}{<DOI(optional, without https://doi.org/)>}{<other comments(optional)>}` | Preprint entry, must be used within `paperlist` environment |
| `\conference{<author>}{<title>}{<conference>}{<location>}{<date>}{<URL(optional)>}{<other comments(optional)>}` | Conference paper entry in `paperlist` environment |
| `\chapter{<author>}{<chaptertitle>}{<editor(optional)>}{<booktitle>}{<edition(optional)>}{<location(optional)>}{<publisher>}{<year>}{<page>}{<URL(optional)>}{<other comments(optional)>}` | Book chapter entry in `paperlist` environment |
| `prelist` environment             | List of presentations |
| `\keynote{<title>}{<conference>}{<location>}{<date>}{<URL(optional)>}{<other comments(optional)>}` | Keynote presentation entry in `prelist` environment |
| `\guest{<title>}{<conference>}{<location>}{<date>}{<URL(optional)>}{<other comments(optional)>}` | Guest presentation entry in `prelist` environment |
| `\oral{<title>}{<conference>}{<location>}{<date>}{<URL(optional)>}{<other comments(optional)>}` | Oral presentation entry in `prelist` environment |
| `\poster{<title>}{<conference>}{<location>}{<date>}{<URL(optional)>}{<other comments(optional)>}` | Poster presentation entry in `prelist` environment |
| `text` environment                | Text description environment, for all other descriptions that are not in brackets |

**NOTE** 

The optional URL / DOI links for papers / presentations, if specified, will turn the paper / presentation title into a hyperlink.
See the example tex files for further details.