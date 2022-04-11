BXorigcapt Package
==================

LaTeX: To retain the original caption names when using Babel

This package forces the caption names (`\chaptername`, `\today`, etc)
declared by the document class in use to be used as the caption names
for a specific language introduced by the Babel package.

Starting from version 0.3, this package also supports Polyglossia.
                                                            
### System requirement

  * TeX format: LaTeX.
  * TeX engine: Any engine with e-TeX extension.
  * Dependent packages:
      - babel or polyglossia
      - etoolbox v2.1+

### Installation

  - `*.sty` → $TEXMF/tex/latex/BXorigcapt

### License

This package is distributed under the MIT License.


The bxorigcapt Package
----------------------

See the manual bxorigcapt.pdf for detail.


Revision History
----------------

  * Version 1.0  〈2022/04/10〉
      - Now e-TeX and etoolbox are required.
      - Add option `main`.
  * Version 0.4a 〈2022/04/08〉
      - Add option `nowarn`.
      - Bug fix.
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
