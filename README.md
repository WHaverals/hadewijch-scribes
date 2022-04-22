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

### Diachronic scribal differences

Finally, there is the question of diachronic differences between Ms. A and Ms. B. We see two options here:

1. The difference between exemplar (Ms. A) and copy (Ms. B) grew larger as the copy progressed. This would imply that the scribe first was very cautious and precise, and only gradually gained confidence before he started diverging more strongly towards the end of the copy.
2. The differences between exemplar and copy grew smaller over time: this would mean that the scribe initially had a very different orthographic profile, but then gradually became "indoctrinated" by his copy .
3. The third option is that... nothing happened. Then we would get a straight line or complete chaos.

Schematically, these options can be represented as follows:

![Alt text](/slides/diachronic_trends.jpeg?raw=true "Possible diachronic trends")

For our analysis we used character tetra- and pentagrams, trying to tease out difference that relate to orthography. The resulting curve is presented below. For every position on the horizontal axis we calculate the stylistic distance (the cosine distance) between two corresponding passages in A and B.
 
![Alt text](/gfx/distance_regression.png?raw=true "Scribal distance")

At face value, it would seem like there is an increase in the distance between both copies. To explore this a bit further, we fitted a linear regression to these points, which clearly shows the increasing trend. Interestingly, it would *seem* that the scribe of Ms. B was very cautious in the beginning and also kept closer to the exemplar’s orthography than near the end of the manuscript. Other than that we see a fairly linear increase with a clear peak in the divergence right before the end.

This would suggest at face value that there is evidence for the hypothesis saying that the scirbe of Ms. B would only gradually diverge from his exemplar, but remained very faithful in the beginning of the copy. However, that would be an oversimplification of the reality. Here, we add some vertical bars to the plot, signaling specific events in the text (shifts in the content and scribal takeovers in Ms. A). As it becomes clear, these "events" coincide with aspects of the curve. The first red vertical line, for instance, shows the point where Ms. A has the first scribal takeover. Thus, instead of assuming that the scribe of Ms. B stayed very close to his exemplar in the first folio’s of the transcriptions, we could also hypothesise that B’s spelling profile just happened to be closer to that of the first scribe in A. We see the same thing after the purple line, that signals the next scribal takeover in Ms. A. Interestingly, this is also a case of serendipity perhaps: whereas our original focus was on Ms. B, we believe this analysis actually tells us more about Ms. A.

![Alt text](/gfx/dist.png?raw=true "Scribal distance")
