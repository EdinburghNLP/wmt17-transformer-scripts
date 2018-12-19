WMT17 TRAINING SCRIPTS
----------------------

We used various different approaches for preprocessing
and data augmentation for monolingual data for different
languages. Check the system description for more detail.

In this directory, we provide a sample configuration for
preprocessing and training for English->German. It is different
from our WMT17 submission in some aspect, most importantly using
the Transformer-base architecture instead of an RNN.

Note that our WMT17 submission uses also
rely on the use of back-translated monolingual data, and
combination of multiple models. Please also have a look at last year's
accompanying scripts and sample configurations; among others,
there is documentation for right-to-left reranking:
https://github.com/rsennrich/wmt16-scripts

USAGE INSTRUCTIONS
------------------

1. ensure that all requirements are present, and that the path names in the ‘vars’ file are up-to-date. If you want to train on GPUs, you should also update the ‘device’ variable in that file.

2. download sample files (WMT17 parallel training data, dev and test sets):

   ```
   scripts/download_files.sh
   ```

3. preprocess the training, development and test corpora:

    ```
    scripts/preprocess.sh
    ```

4. train a Nematus model:

    ```
    scripts/train.sh
    ```

5. evaluate your model:

    ```
    scripts/evaluate.sh
    ```

