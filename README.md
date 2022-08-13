# Summary

This Universal Dependencies (UD) Japanese treebank is based on the definition of
UD Japanese convention described in the UD documentation.
The original sentences are from `Balanced Corpus of Contemporary Written Japanese'(BCCWJ).

UD-Japanese-BCCWJLUW is the other word segmentation version of UD-Japanese-BCCWJ.
We use **Long Unit Word (LUW)** as their syntactic word in UD definition.

# Introduction

The Japanese UD treebank contains the sentences from BCCWJ [1]
https://clrd.ninjal.ac.jp/bccwj/en/
with BCCWJ-DepPara[2] annotation.

The word units is based on **Long Unit Word** in BCCWJ [1].
We prepared conversion rules from BCCWJ-DepPara to UD_Japanese v2.1 guidelines [3][4].

## Recovering data

The data is provided in the CoNLL format, but original texts are
stripped off due to the license issue.

The corpus is obtained by running the following command:

```
./merge/merge.sh -c BCCWJ_CORE_FILE
```

where `BCCWJ_CORE_FILE` denotes the file of BCCWJ core file (core_LUW.txt, OT) 
the script requires Python (3.x)

or

The BCCWJ DVD edition purchaser can download the data with the original text
from https://bccwj-data.ninjal.ac.jp/

## Spliting

Each data set contains UD annotations for the following parts in BCCWJ

training: annotation B, C, D, E subsets
development: annotation A subset
test: annotation A subset

See also https://github.com/masayu-a/BCCWJ-ANNOTATION-ORDER

# Acknowledgments

The original treebank was provided by:

- National Instutite for Japanese Language and Linguistics, Japan

The corpus was converted by:

- Mai Omura
- Aya Wakasa
- Masayuki Asahara

through annotation, discussion and validation with

- Kayo Yamashita

This work was supported by JSPS KAKENHI Grants Numbers JP17H00917
and NINJAL Annotation Project.

# License

See file LICENSE.txt

# Reference

[1] Maekawa, K., Yamazaki, M., Ogiso, T., Maruyama, T., Ogura, H., Kashino, W.,
Koiso, H., Yamaguchi, M., Tanaka, M. & Den, Y. (2014). Balanced corpus of contemporary written Japanese. Language resources and evaluation, 48(2), 345-371.
[2] Asahara, M., & Matsumoto, Y. (2016). Bccwj-deppara: A syntactic annotation treebank on the 'Balanced Corpus of Contemporary Written Japanese'. In Proceedings of the 12th Workshop on Asian Language Resources (ALR12) (pp. 49-58).
[3] Tanaka, T., Miyao, Y., Asahara, M., Uematsu, S., Kanayama, H., Mori, S., &
Matsumoto, Y. (2016). Universal Dependencies for Japanese. In LREC-2016.
[4] Asahara, M., Kanayama, H., Tanaka, T., Miyao, Y., Uematsu, S., Mori, S.,
Matsumoto, Y., Omura, M., & Murawaki, Y. (2018). Universal Dependencies Version 2 for Japanese. In LREC-2018.

Changelog
2022-11-01   v2.10 **(UD_Japanese-BCCWJLUW)**
  * Update v2.10 to v2.11
2022-05-01   v2.10 **(UD_Japanese-BCCWJLUW)**
  * Update v2.9 to v2.10
2021-11-01   v2.9 **(UD_Japanese-BCCWJLUW)**
  * Initial release in Universal Dependencies.
2021-05-01   v2.8 (UD_Japanese-BCCWJ)
  * Update v2.7 to v2.8
2020-11-01   v2.7 (UD_Japanese-BCCWJ)
  * Update v2.4 to v2.7
2019-05-01   v2.4 (UD_Japanese-BCCWJ)
  * Update v2.3 to v2.4.
2018-11-01   v2.3 (UD_Japanese-BCCWJ)
  * Update v2.2 to v2.3.
2018-03-28   v2.2 (UD_Japanese-BCCWJ)
  * Initial release in Universal Dependencies.

<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.9
License: CC BY-NC-SA 4.0
Includes text: no
Genre: news nonfiction fiction blog web
Lemmas: not available
UPOS: converted from manual
XPOS: not available
Features: not available
Relations: converted from manual
Contributors: Omura, Mai; Asahara, Masayuki; Miyao, Yusuke; Tanaka, Takaaki; Kanayama, Hiroshi; Matsumoto, Yuji; Mori, Shinsuke; Uematsu, Sumire; Murawaki, Yugo
Contributing: elsewhere
Contact: masayu-a@ninjal.ac.jp
===============================================================================
</pre>
