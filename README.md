Notes:
The reduced tones are splitted into three types (according to the phoneset of the pretrained model):

tone 6: reduced tone after tone 1 and tone 2;

tone 7: after tone 3;

tone 8: after tone 4.

Still, tone 5 stands for all sorts of reduced tones. In the dictionary, a pinyin label with tone 5 has the same possibility to fall into each kind.

Example of tone 6-8:

太 高 了 : tai4  gao1  le6

我的 : wo3 de7

我干的 : wo3 gan4 de8

Example of using in the alignment:

Run in terminal:

mfa align path/to/input/corpus/folder path/to/this/dictionary/mandarin_pinyin_to_mfa_lty.dict mandarin_mfa path/to/output/folder 
