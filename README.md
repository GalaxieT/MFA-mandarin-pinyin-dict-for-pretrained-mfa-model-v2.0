请注意，本字典**不**适用于mfa 3.0版本的模型（#8 ）
Cannot work with model v3.0 (#8)

Related project: [Montreal-Forced-Aligner](https://github.com/MontrealCorpusTools/Montreal-Forced-Aligner)

A dictionary for Montreal-Forced-Aligner users to align mandarin data labeled in pinyin form using the mfa pretrained acoustic model v2.0.

适用于Montreal-Forced-Aligner的汉语普通话对齐中，以拼音标注为输入，并调用MFA预训练声学模型V2.0的情况。

Notes:
The reduced tones are splitted into three types (according to the phoneset of the pretrained model):

tone 6: reduced tone after tone 1 and tone 2;

tone 7: after tone 3;

tone 8: after tone 4.

Still, tone 5 stands for all sorts of reduced tones. In the dictionary, a pinyin label with tone 5 has the same possibility to fall into each kind.

Example of tone 6-8:

太 高 了 : tai4  gao**1**  le**6**

我 的 : wo**3** de**7**

我 干 的 : wo3 gan**4** de**8**

Example of using in the alignment:

Run in terminal:

`mfa align path/to/input/corpus/folder path/to/this/dictionary/mandarin_pinyin_to_mfa_lty.dict mandarin_mfa path/to/output/folder `

简单来说，MFA按照轻声的上一个音的声调，把轻声分为三类。如果输入标注中不想分这么细的话，可以直接输入5，代表有相等可能属于这三类中的每一类。
