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

- [iKF1028](sbml/iKF1028): Stoichiometric balance corrections in
  [8791efa](https://github.com/zhanglab/psamm-model-collection/commit/8791efa58d0b01a06384b03ce11a6fcbc03fe8c3).
- [iSyn731](sbml/iSyn731): Updated to new model from http://www.maranasgroup.com/models.htm
  downloaded on September 9, 2015 (changes:
  [ca39f98](https://github.com/zhanglab/psamm-model-collection/commit/ca39f98172275718bdbc369c53015b71aec91e70)).
