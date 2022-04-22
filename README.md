# Hadewijch Scribal Analysis

Repository containing code and data for talk at the international workshop 'On the way to the future of digital manuscript studies' 
(27-29 October 2021, Radboud Universiteit Nijmegen) [article forthcoming]

### Hadewijch's oeuvre

The oeuvre of the medieval mystic Hadewijch (13th century) has been fully preserved in three manuscripts, commonly referred to as 'A', 'B' and 'C', with A and B being the two oldest Hadewijch manuscripts:

- Manuscript A is dated in the first half of the fourteenth century, more specifically 1325-1350. Previous research has shown that three scribes were responsible for copying the text. 

- Manuscript B is dated around 1380. The consensus is that the scribe responsible for copying Ms. B used Ms. A as an exemplar.

With Ms. B being, supposedly, a direct copy of Ms. A, we have a very rare case in Middle Dutch philology.

![Alt text](/slides/A_B.jpeg?raw=true "Hadewijch Manuscripts A and B")

In terms of content, mss. A and B contain the same texts. Also the order of texts is preserved:

1. Letters
2. Visions
3. Songs
4. Poems
5.  -- Ms. B also contains additional poems at the end, which are not considered part of Hadewijch's oeuvre) --

![Alt text](/slides/texts.jpeg?raw=true "Order of texts in mss. A and B")

### Materials used

- Detailed, hyperdiplomatic transcriptions of the Letters of Hadewijch in both manuscripts (ca. 1/3 of textual material)
- Using _Transkribus_, we automatically transcribed the rest of both manuscripts (CER < 2.5%)

### Stylometry for scribal analysis

*Research question: Can we model how one scribe appropriated his exemplar?*

Using conventional methods from stylometry -- or the quantitive study of writing style -- we analysed scribal writing styles.

From the first graph below, we explore the most discriminative constrasts in word use between the manuscripts as a whole. Especially striking here is the use of abbreviations in ms. B (whereas in ms. A, the full variant of the word is often written out). Already from this preliminary result, we can conclude that the appropriation of the exemplar is real, and -- moreover -- consistent enough to be modelled quantitatively.

![Alt text](/gfx/zeta.png?raw=true "Zeta for Scribal Analysis")

Next, we investigated the difference between both manuscripts on the basis of character n-grams. The graph shows the discriminative orthographic variants between the two manuscripts. In Ms. B, we find, among others: 

- the insertion of the character «h» (e.g. «ghenoech», «heilighen») where it isn't necessary, strictly speaking. 
- the use of «u» instead of «v», and not only in intravocalic positions. 
- word-initial «z-», where «s-» is more common in Ms. A.

![Alt text](/gfx/features.png?raw=true "Zeta for Scribal Analysis")

 



![Alt text](/gfx/dist.png?raw=true "Scribal distance")
