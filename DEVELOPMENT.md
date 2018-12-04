AP Computer Science A Curriculum Development
====================================================================================================

Versioning
----------
For purposes of versioning, we will be using _major_._minor_._patch_ notation. For now, we'll keep
the exact definitions of each fuzzy, which is particularly appropriate given that we're mostly
talking about documentation as opposed to software (what's a “breaking change” in documentation?).
Versions will come up with Git tags, change logs, and possibly releases (such as zip archives).

Generally, _patch_ numbers increase on minor updates, such as formatting, typos, or minor content
updates.

_Minor_ numbers increase as new content is added.

_Major_ number increase as content undergoes a large-scale update. For example, when the repo has
finished conversion from Word & PowerPoint curriculum content, we'll upgrade from 1.x.x to 2.0.0.


Tools
-----
Several tools were/are used in the development of this content. See the [Tools Notes] for more
information.

In addition to the standalone tools, there's a simple `make.cmd` file in the root of the project
used to run common tasks. Right now, all it does is build all PDFs from source Word .docx files.
This uses the `tools\docto.exe` utility. The command `make pdfs` will create new PDF files from any
changed `.docx` files listed in the `docx.manifest` file. Note that for some reason, `docto` does
not properly handle the three files `Unit6\Text Excel [ABC] Student Guide.docx`. These have been
removed from the `docx.manifest` file, and must be saved as PDF manually.

Run `make help` for any other usage information.



[Tools Notes]: ../tools/README.md
