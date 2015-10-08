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

- [iJN746](sbml/iJN746): Corrected compound references to cardiolipins in biomass reaction
  to refer to cardiolipins in the periplasm:
  [7d68a62](https://github.com/zhanglab/psamm-model-collection/commit/7d68a6236faf5835229971cbc84cc2eab36ca1fa).
