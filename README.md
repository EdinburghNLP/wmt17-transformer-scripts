# WMT17 TRANSFORMER SCRIPTS
-------------------------------------------

This is a fork of https://github.com/EdinburghNLP/wmt17-scripts that
demonstrates training of Nematus models with a Transformer architecture.

`training/scripts/train.sh` shows a configuration corresponding to training a Transformer-base model.

Scripts for preprocessing, validation, and evaluation, are also provided, and mirror the WMT17 setup
of the University of Edinburgh (with minor tweaks, e.g. reducing the BPE vocabulary size).

REQUIREMENTS
------------

The models use the following software:

 - moses decoder (scripts only; no compilation required) https://github.com/moses-smt/mosesdecoder
 - nematus: https://github.com/EdinburghNLP/nematus
 - subword-nmt https://github.com/rsennrich/subword-nmt

Please set the appropriate paths in the 'training/vars' file.


USAGE INSTRUCTIONS
------------------------------------

For training, follow the instructions in `training/README.md`

LICENSE
-------

All scripts in this directory are distributed under MIT license.
