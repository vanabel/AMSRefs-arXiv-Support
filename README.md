# AMSRefs arXiv Support

This repository provides enhanced arXiv support for AMSRefs bibliography styles. It includes modified versions of the standard AMSRefs .bst files to properly handle arXiv references.

## Modified Bibliography Styles

- `amsra.bst` - Alphabetic style
- `amsrn.bst` - Numeric style (default)
- `amsrs.bst` - Short alphabetic style
- `amsru.bst` - Citation-order style

## Usage

1. Copy the desired .bst file to your TeX project
2. Use the appropriate style option in your document:
   ```latex
   \usepackage[abbrev,msc-links,backrefs]{amsrefs}  % numeric (default)
   \usepackage[alphabetic,abbrev,msc-links,backrefs]{amsrefs}  % alphabetic
   \usepackage[shortalphabetic,abbrev,msc-links,backrefs]{amsrefs}  % short alphabetic
   \usepackage[citation-order,abbrev,msc-links,backrefs]{amsrefs}  % citation-order
   ```

## Example

See `test.tex` for a working example. 