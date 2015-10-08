PSAMM model collection
======================

This is a collection of published GEMs that have been converted to the file
format used by [PSAMM](https://github.com/zhanglab/psamm), using the
[psamm-import tool](https://github.com/zhanglab/psamm-import).

The collection of models is split into two sections:

- [**sbml**](sbml): Models that have been loaded as SBML files using the _sbml_
  loader in _psamm-import_.
- [**excel**](excel): Models that have been loaded using a model-specific Excel
  file loader in _psamm-import_.

Model corrections
-----------------

- [iRsp1095](sbml/iRsp1095): Changed medium for growth based on medium description in
  [Imam et al. 2011](https://doi.org/10.1186/1752-0509-5-116):
  [3340d7a](https://github.com/zhanglab/psamm-model-collection/commit/3340d7a476485a6e22f77a0561a803b4281d2615).
