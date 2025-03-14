# AMSRefs arXiv Support

This repository provides enhanced arXiv support for AMSRefs bibliography styles. It includes modified versions of the standard AMSRefs .bst files to properly handle arXiv references.

## Preview

![arXiv Reference Styles](arXiv-style-Reference.png)

## Modified Bibliography Styles

- `amsra.bst` - Alphabetic style
- `amsrn.bst` - Numeric style (default)
- `amsrs.bst` - Short alphabetic style
- `amsru.bst` - Citation-order style
- `amsry.bst` - Year y2k style

## Usage

1. Copy the desired .bst file to your TeX project
2. Use the appropriate style option in your document:
   ```latex
   % Required for backrefs support
   \usepackage[backref=page]{hyperref}
   
   \usepackage[abbrev,msc-links,backrefs]{amsrefs}  % numeric (default)
   \usepackage[alphabetic,abbrev,msc-links,backrefs]{amsrefs}  % alphabetic
   \usepackage[shortalphabetic,abbrev,msc-links,backrefs]{amsrefs}  % short alphabetic
   \usepackage[citation-order,abbrev,msc-links,backrefs]{amsrefs}  % citation-order
   \usepackage[alphabetic,y2k,abbrev,msc-links,backrefs]{amsrefs}  % year style (must use with alphabetic)
   ```

## Example

See `test.tex` for an example of how to use the styles.