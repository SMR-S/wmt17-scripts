WMT17 TRAINING SCRIPTS
----------------------

We used various different approaches for preprocessing
and data augmentation for monolingual data for different
languages. Check the system description for more detail.

In this directory, we provide a sample configuration for
preprocessing and training for English->German. Please note
that this script will not reproduce our WMT17 results, which also
rely on the use of back-translated monolingual data, and
combination of multiple models. Please also have a look at last year's
accompanying scripts and sample configurations; among others,
there is documentation for right-to-left reranking:
https://github.com/rsennrich/wmt16-scripts


USAGE INSTRUCTIONS
------------------

1. download sample files (WMT17 parallel training data, dev and test sets):

   ```
   scripts/download_files.sh
   ```

2. preprocess the training, development and test corpora:

    ```
    scripts/preprocess.sh
    ```

3. train a Nematus model:

    ```
    scripts/train.sh
    ```

4. evaluate your model:

    ```
    scripts/evaluate.sh
    ```
