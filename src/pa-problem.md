# Pairwise alignment problem

Comparing two text sequences is one of the most basic tasks with data. If the
sequences have no mistakes, then sequence \\(A\\) can be aligned to sequence \\(B\\)
letter-to-letter without mistakes between the aligned letters. Such an alignment
can be made by iterating through the corresponding word letters just once and
checking if they match.

TODO: image of an exact global alignment

In many real-world applications, though, errors happen and our alignment
algorithm has to tolerate them. If letters can be substituded, our alignment may
include mismatching letters that are aligned to each other. The number of such
mistamches is called _Hamming distance_ between \\(A\\) and \\(B\\)---counting
them only takes one pass through the sequences. It is often useful for
bit-sequences.

TODO: image of an global alignment with hamming distance = 2

What if letters may be not only substituted, but also inserted or deleted? Now
aligning is not streigh-forward anymore since there are many possible
alignments, each including different number of mismatching corresponding
letters.

TODO: 2 images of global alignments with different Levenshtein distances

Among all alignments, we can try finding one that minimizes the number of
necessary edits (subsitutions, insertions and deletions). The minimal number of
such edits needed to convert \\(A\\) to \\(B\\) is called _Levenshtein distance_. Note
that converting \\(B\\) to \\(A\\) takes the same number of edits.

We can generalize the Levenshtein distance to different _costs_ of the edit
operations, e.g. subtitutions may each cost \\(1\\) but gaps (i.e. insertions and
deletions) may cost \\(5\\).

TODO: An alignment with edit distance
