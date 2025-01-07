Data Formatting for Collaboration
=================================

Introduction
---------------------------------
When collaborating with the Qoroyo team, it is essential to format your data correctly. 
Proper formatting ensures that your texts can be displayed alongside other texts as well as the accompanying word level analyses.
This section provides guidelines on how to structure your data for optimal compatibility with Qoroyo's tools and systems.

Data structure Biblical texts
----------------------------------
Hebrew and Syriac need to follow the ETCBC transliteration schema. You can find these schemas here: :ref:`HEB` and :ref:`SYR`.

Files should be plain-text with four columns. Where each column is separated by a tab.

.. list-table:: File structure
   :class: chars
   :widths: auto
   :header-rows: 1

   * - ID 
     - Bible identifier
     - Token
     - Encoded token (optional)
   * - Only for personal reference, will be ignored by Qoroyo
     - Bookname abbreviation chapter number verse number--each separated by a space
     - Word/wordgroup [#f1]_
     - (Optional) ETCBC encoding manually applied or predicted by AI [#f2]_

For example, Peshitta Exodus will be encoded in a text file as follows: 

.. code-block::
   :caption: Exodus 1 1

        0	Ex 1 1	WHLJN	W-HLJN
        1	Ex 1 1	CM"H>	CM&H/(J~>
        2	Ex 1 1	DBN"J	D-BN/J
        3	Ex 1 1	>JSRJL	>JSRJL/
        4	Ex 1 1	D<LW	D-<L(L[W
        5	Ex 1 1	LMYRJN	L-MYRJN/
        6	Ex 1 1	<M	<M
        7	Ex 1 1	J<QWB	J<QWB/
        8	Ex 1 1	GBR	GBR/
        9	Ex 1 1	WBJTH	W-BJT/-H
        10	Ex 1 1	<LW	<L(L[W
        11	Ex 1 2	RWBJL	RWBJL/
        12	Ex 1 2	WCM<WN	W-CM<WN/
        ...
        16334	Ex 40 38	>JSRJL	>JSRJL/
        16335	Ex 40 38	BKL	B-KL/
        16336	Ex 40 38	MC"QLNJHWN	MCQLN/J-HWN        

.. rubric:: Footnotes
.. [#f1] e.g., BRCJT (barashit) is composed of multiple words (preposition and noun), however in Hebrew it is written together; hence, it is considered a single token and should be written as such.
.. [#f2] e.g., The aforementioned BRCJT will now be properly demarcated to contain preposition and noun via special characters: B-RCJT/
