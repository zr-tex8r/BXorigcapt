BXorigcapt Package
==================

LaTeX: To retain the original caption names when using Babel

This package forces the caption names (`\chaptername`, `\today`, etc)
declared by the document class in use to be used as the caption names
for a specific language introduced by the Babel package.

Starting from version 0.3, this package also supports Polyglossia.
                                                            
### System requirement

  * TeX format: LaTeX.
  * TeX engine: Anything.
  * Dependent packages:
      - babel or polyglossia

### Installation

  - `*.sty` → $TEXMF/tex/latex/BXorigcapt

### License

This package is distributed under the MIT License.

The bxorigcapt Package
----------------------

### Introduction

Suppose you have designed a document class tailored for the Esperanto
language. The class has the following definition of caption names and you
like it:

    \newcommand\contentsname{Tabelo de Enhavo}

If a document is written solely in Esperanto, then there is no need to
employ the Babel package. (Yes, the document class should select the
hyphenation rule for the language.)  However, when you want to create
document that contains Esperanto and German, then you have to utilize
Babel, to have correct hyphenations for both languages.

    \usepackage[ngerman,esperanto]{babel}

But unfortunately, this changes `\contentsname` from “Tabelo de Enhavo”
(what you have chosen) to “Enhavo” (what is declared in the language
definition file of Babel), which is unfavorable.

In fact, when using a document class for a specific language, the most
suitable caption names *for that language* should be the ones provided by
the class. The bxorigcapt package realizes this natual request, that is,
it enables you to make the caption names declared in the current document
class treated as the caption names for a specific language.

### Package Loading

    \usepackage[<option>,...]{bxorigcapt}

Available options are:

  - a Babel language name: Specifies the target language. The default
    target language is the main language of Babel.
  - `warn`: Issues a warning (instead of an info) if Babel is never
    loaded in the preamble.

### Usage

Once this package is loaded, the caption names provided by the document
class (actually the ones that are effective when this package is loaded)
will be used as the caption names for the target language (which is
specified by the package option).

This package has no public commands.


Revision History
----------------

  * Version 0.4  〈2022/03/12〉
      - Adjustment for new version of Babel.
      - Add option `warn`.
  * Version 0.3  〈2018/09/05〉
      - Add support for Polyglossia.
  * Version 0.2a 〈2017/05/03〉
      - Minor fix.
  * Version 0.2  〈2016/04/01〉
      - The first public version.

--------------------
Takayuki YATO (aka. "ZR")  
https://github.com/zr-tex8r
