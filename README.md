# grapheme-to-phoneme

### projects
* [multilingual-chinese-transformer](https://github.com/kakaobrain/g2pM)
* [multilingual-opennmt](https://github.com/bpopeters/mg2p)
* [sequitur](https://github.com/sequitur-g2p/sequitur-g2p)
* [uni-saarland](https://github.com/akshayjoshii/Speech-Recognition)
* [pointer-generator](https://github.com/nala-cub/g2p-pgt)

* [sigmorphon](https://sigmorphon.github.io/sharedtasks/2020/)
    * [paper](https://www.aclweb.org/anthology/2020.sigmorphon-1.2.pdf)
    * [sigmorphon2020-github](https://github.com/sigmorphon/2020)
    * [poster+papers](https://sigmorphon.github.io/workshops/2020/shared_tasks/)

    * data: `There are 3600 training data examples and 450 development and test data examples for each language`
    * method: (baseline) 
        * `single-layer bidirectional LSTM encoder and a single-layer unidirectional LSTM decoder connected using an attention mechanism [...] using the fairseq library`
        * ` We use the development set to tune—for each language—batch size (256, 512,1024), dropout (.1, .2, .3), and the size of the encoder and decoder modules`
            -> WTF! 256 batch-size is way too big!
        * `A module is said to be “small” when it has a 128-dimension embedding layer and a 512-unit hidden layer, and “large” when it has a 256-dimension embedding layer and a 1024-unit hidden layer.`

* [CMUS-Sphinx](https://cmusphinx.github.io/2016/04/grapheme-to-phoneme-tool-based-on-sequence-to-sequence-learning/)
    * [github](https://github.com/cmusphinx/g2p-seq2seq)
        * data: [cmudict](https://github.com/cmusphinx/cmudict)
        * method: Transformer num_layers=3, size=256
        
* [JOINTLY LEARNING TO ALIGN AND CONVERT GRAPHEMES TO PHONEMESWITH NEURAL ATTENTION MODELS](https://arxiv.org/pdf/1610.06540v1.pdf)
    * data: 
        * CMUDict data: train/test = 106,837/12,000-word
        * Pronlex data: train/dev/test-set =  83,182/2,400/4,800 words
        * NetTalk data: train/test = 14,851/4,951 words
    * method: 
        * stacked LSTMs, 3 layers, each with 512 units; 512-dimensional embedding vectors for characters and  the  phonemes

### data
* [IPA](https://github.com/open-dict-data/ipa-dict)
* [cmudict](https://github.com/cmusphinx/cmudict)
* [wikipron](https://github.com/kylebgorman/wikipron)
