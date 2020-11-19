# Multilingual-QA-Based-On-BERT

## Usage:

* simply implement on [Colab](http://colab.research.google.com)

### BERT_MLQA:

* How to download [MLQA](https://github.com/facebookresearch/MLQA) dataset:

```Bash
pip install gdown
sudo apt-get install unzip
gdown https://dl.fbaipublicfiles.com/MLQA/MLQA_V1.zip
unzip MLQA_V1.zip
rm MLQA_V1.zip
```

* Python packages to install:

```Bash
pip install transformers
```
### [Fast_Align](https://github.com/clab/fast_align):

* How to set up the dependencies:

```Bash
git clone https://github.com/clab/fast_align.git
sudo apt - get install libgoogle - perftools - dev libsparsehash - dev
cd fast_align
mkdir build
cd build
cmake ..
make
```

* How to implement a sample text:

```Bash
echo "doch jetzt ist der Held gefallen . ||| but now the hero has fallen ." >> sample.txt
echo "neue Modelle werden erprobt . ||| new models are being tested ." >> sample.txt
echo "doch fehlen uns neue Ressourcen . ||| but we lack new resources ." >> sample.txt

./fast_align -i sample.txt -d -o -v > forward.align
cat forward.align
```
### BERT_MLQA_MUSE:

* Download [MLQA](https://github.com/facebookresearch/MLQA) dataset.

* Python packages to install:

```Bash
pip install opencc
pip install transformers
```
