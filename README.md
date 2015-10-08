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
- [iKF1028](sbml/iKF1028): Stoichiometric balance corrections in
  [8791efa](https://github.com/zhanglab/psamm-model-collection/commit/8791efa58d0b01a06384b03ce11a6fcbc03fe8c3).
- [iRsp1095](sbml/iRsp1095): Changed medium for growth based on medium description in
  [Imam et al. 2011](https://doi.org/10.1186/1752-0509-5-116):
  [3340d7a](https://github.com/zhanglab/psamm-model-collection/commit/3340d7a476485a6e22f77a0561a803b4281d2615).
- [iSyn731](sbml/iSyn731): Updated to new model from http://www.maranasgroup.com/models.htm
  downloaded on September 9, 2015 (changes:
  [ca39f98](https://github.com/zhanglab/psamm-model-collection/commit/ca39f98172275718bdbc369c53015b71aec91e70)).
- [RECON2](sbml/recon2): Fix stoichiometric consistency:
  [5671060](https://github.com/zhanglab/psamm-model-collection/commit/5671060606674cec61141f71dbe0d9d545e149dc).
