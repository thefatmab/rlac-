---
title: "Assignment 1: Institutional Language and Narrative Power in Harry Potter Canon and Fan Fiction"
layout: archive
permalink: /assignments/
author_profile: true
---

## Introduction

In what ways does power move between fan-made and canonical narratives? Do fan fiction works replicate and reinterpret institutional authority, or do they undermine it? Prior to starting this study, we believed that fan fiction would place more focus on human agency, interpersonal relationships, and decision-making, whereas official Harry Potter novels would prioritize institutional authority Hogwarts, academics, and the Ministry of Magic. Our working hypothesis was that fan fiction would have a greater proportionate frequency of language connected to agency, whereas canon would be dominated by linguistic indications of institutional authority.

We created a five-text corpus of three fan fiction pieces (Twin Sister, Adoptive Kaiju, and Resurrection) and two canonical novels (Harry Potter and the Sorcerer's Stone and Harry Potter and the Deathly Hallows) in order to verify this hypothesis. First, using Voyant Tools for exploratory remote reading and RMarkdown in posit. We examined the distribution and relative frequency of words connected to institutions and agencies throughout the corpus using cloud for structured lexical comparison.

The anticipated conflict between canon and fandom is complicated by what unfolded. Even in transformational fan tales, institutional authority continues to play a major role in vocabulary. Fan fiction seems to restructure institutional authority inside modified narrative frameworks rather than substituting simply individualistic autonomy for formal power frameworks.

## Corpus and Methodological Design

This project combines exploratory and confirmatory computational methods. Voyant Tools enabled rapid visualization of word frequency (Cirrus), term trends across documents, and keyword distribution (Bubblelines). These tools function as exploratory instruments, surfacing patterns that may not be immediately visible through linear reading.
RMarkdown was then used to tokenize the corpus, remove stopwords, normalize word frequencies, and group selected terms into conceptual categories. Following the explanation in Hermeneutica, Chapter 2 (“How Computers Measure Words”), computational text analysis operates by abstracting literature into tokens. Words become measurable units divorced from syntactic and narrative context. This transformation makes cross-text comparison possible, but it also risks oversimplifying meaning.
To examine how authority circulates, we constructed two lexical categories:
Institutional terms: dumbledore, professor, ministry, headmaster, authority
Agency terms: choose, decide, control, plan, trust, love
These categories allowed structured comparison across texts while remaining aware that lexical grouping is itself an interpretive act.

## Voyant Insights: Lexical Prominence and Structural Authority

Figure 1: Cirrus Word Cloud
The Cirrus word cloud reveals that “dumbledore” appears prominently across the corpus. Institutional markers such as “professor” and “ministry” are also visually dominant, particularly in canonical texts. Interestingly, in Twin Sister, character-specific names rise to prominence, signaling a shift toward identity-centered reinterpretation.
The word cloud confirms that authority figures remain lexically central across both canon and fan fiction. However, prominence alone does not indicate whether authority is affirmed, questioned, or reconfigured. 

![Figure 1: Word Cloud]({{ site.baseurl }}/assets/images/fig1-voyant-wordcloud.png)
Figure 1. Most frequent terms across the five-text corpus (Voyant Cirrus).

## Figure 2: Term Trends
The Trends graph compares selected keywords across documents. Several patterns emerge:
“Dumbledore” peaks dramatically in Deathly Hallows.

“Professor” is most concentrated in Sorcerer’s Stone.

“Family” spikes significantly in Twin Sister.

“Plan” remains relatively moderate across texts.

These patterns suggest that canonical texts foreground institutional structures, while fan fiction introduces relational language. However, the persistence of institutional terms in fan works challenges the assumption that fan fiction dismantles authority outright.
The Trends visualization reveals something that close reading might not quantify easily: structural continuity across textual transformations.

![Figure 2: Term Trends]({{ site.baseurl }}/assets/images/fig2-trends.png)
Figure 2. Relative frequency of selected keywords across canonical and fan fiction texts.

## Figure 3: Bubblelines (Dumbledore Distribution)
The Bubblelines visualization shows how frequently and how consistently “dumbledore” appears across documents. In Deathly Hallows, references cluster densely throughout the narrative. In Twin Sister and Adoptive Kaiju, the term appears with notable consistency rather than marginal presence.
This is a crucial finding. If fan fiction sought to displace institutional authority, we might expect diminished lexical centrality of key authority figures. Instead, authority persists lexically.
Yet frequency does not capture tone. As Kestemont and Herman argue in “Can Computers Read (Literature)?”, computational tools measure textual features but cannot interpret irony, skepticism, or critique. A frequent name may signal reverence, subversion, or narrative dependency. Distant reading identifies structural presence, not evaluative stance.

![Figure 3: Bubblelines (Canon)]({{ site.baseurl }}/assets/images/fig3-bubblelines.png)
![Figure 3: Bubblelines (Fan Fiction)]({{ site.baseurl }}/assets/images/fig3-2bubblelines.png)
Figure 3. Distribution of the term “dumbledore” across the corpus.

## Interactive Voyant Visualization
<iframe style='width: 100%; height: 800px;' src='https://voyant-tools.org/?panels=cirrus%2Creader%2Ctrends%2Csummary%2Ccontexts&corpus=5f1008ebba61f03f42e70984179b2c82'></iframe> 

## R Analysis: Institutional vs. Agency Vocabulary
To move beyond exploratory visualization, we implemented structured comparison in R.
After tokenization and stopword removal, we calculated word counts by text and normalized frequencies per 10,000 words. This normalization accounts for variation in text length, preventing longer works from skewing raw counts.
## Figure 4: Institutional vs. Agency Word Counts
The grouped bar chart shows that institutional vocabulary dominates across canonical texts, particularly Deathly Hallows. Surprisingly, Twin Sister also exhibits strong institutional density. Rather than rejecting authority, this fan text intensifies engagement with it.
Agency markers increase modestly in fan fiction, but not dramatically. The difference is present yet nuanced.
This challenges my initial hypothesis. Fan fiction does not simply replace institutions with individual choice; it repositions authority within altered narrative frameworks.

![Figure 4: Institutional vs Agency Counts]({{ site.baseurl }}/assets/images/fig4-bar.png) 
Figure 4. Comparison of institutional and agency word counts by text.

## Figure 5: Heatmap (Normalized Frequency per 10,000 Words)
The heatmap refines this analysis by normalizing frequencies.
Key observations:
“Dumbledore” frequency remains high even in fan fiction.
“Professor” peaks in Sorcerer’s Stone.
“Family” increases in Resurrection.
Agency markers remain comparatively low overall.
Normalization confirms structural continuity across canon and fandom. Authority is not erased; it is reinterpreted.

![Figure 5: Normalized Frequency Heatmap]({{ site.baseurl }}/assets/images/fig5-heatmap.png)
Figure 5. Normalized keyword frequency (per 10,000 words) across texts.

## What Computational Analysis Reveals
Computational analysis reveals patterns that sequential reading might obscure. It would be difficult to intuitively compare lexical density across five long texts without statistical aggregation. Distant reading exposes proportional emphasis and structural prominence.
However, as Ted Underwood cautions in “The Risks of Distant Reading,” frequency patterns risk overinterpretation. Quantitative prominence does not equal narrative importance. A word may appear rarely yet shape central conflict.
Similarly, corpus composition shapes outcomes. As discussed in class regarding the pitfalls of Google Ngram, shifts in dataset structure influence apparent trends. Our corpus includes both canonical novels and fan fiction, genres that operate under different narrative conventions. Observed differences may reflect genre norms as much as ideological transformation.
Computational tools reveal tendencies, not truths.

## Reading, Fast and Slow
Class discussions of close versus distant reading further contextualize this project. Speed reading and LLM summarization prioritize efficiency; distant reading prioritizes scale. Yet both sacrifice nuance.
Our workflow occupies an intermediate position. Voyant enables rapid pattern recognition, while R enforces deliberate categorization. Unlike large language models, which synthesize narrative probabilistically, this analysis remains transparent: word lists, grouping logic, and normalization methods are explicit.
As “People Don’t Read But LLMs Do” suggests, machine reading identifies statistical regularities rather than interpretive meaning. This project demonstrates both the power and limitation of that approach.

## Scope and Scale
Focused comparison is made possible by restricting the corpus to five works, although generalizability is limited. There may be more noticeable changes in agency language in a bigger corpus of fan fiction. On the other hand, a smaller corpus might mask fandom variations.
Understanding is shaped by scale. Cross-text comparison is made possible by distant reading, but sophistication is restored by close reading. The most effective strategy alternates between them.

## Conclusion
This analysis complicates the assumption that fan fiction displaces institutional authority in favor of personal agency. While relational language increases modestly in fan works, institutional markers particularly references to Dumbledore remain structurally central.
Distant reading reveals continuity where rupture was expected.
Yet computational analysis alone cannot determine whether authority is affirmed or subverted. As Underwood reminds us, distant reading identifies patterns but does not interpret them. Interpretation remains human work.
By pairing Voyant exploration, R-based modeling, and theoretical reflection, this project demonstrates both the utility and the limits of reading like a computer.

## Works Referenced
Underwood, Ted. Distant Horizons: Digital Evidence and Literary Change. Chapter “The Risks of Distant Reading.”

Kestemont, Mike, and Luc Herman. “Can Computers Read (Literature)?”

Hermeneutica. Chapter 2, “How Computers Measure Words.”

“The Pitfalls of Using Google Ngram.”

“People Don’t Read But LLMs Do.”


“READY FOR GRADING!” 


---
## Assignment 2: Signals in the Noise: Comparing Stylo and TF-IDF in a Mid-Century Science Fiction Corpus
---

## Introduction

Science fiction often looks coherent when viewed from a bookstore shelf. Readers expect recurring motifs: spaceships, alien worlds, dangerous inventions, ruined futures, authoritarian governments, time travel, and encounters with the unknown. Because of those repeating conventions, it is easy to assume that science fiction writers of the same era must also write in similar ways. This assignment demonstrates that the assumption is misleading. Once computational methods are applied, the genre becomes much more internally diverse. Writers may share subject matter while differing dramatically in sentence habits, vocabulary, pacing, and thematic emphasis.
This project compares two analytical methods introduced in class: Stylo and TF-IDF. Both examine texts at scale, but they measure different aspects of writing. Stylo, using the R package explored in Posit Cloud, relies heavily on the most frequent words (MFWs) in a corpus. These are usually common grammatical words such as the, and, of, to, and in. Because authors use these words unconsciously and consistently, Stylo is especially useful for identifying stylistic similarity and authorship patterns. TF-IDF, by contrast, reduces the importance of common words and highlights vocabulary that is distinctive within a specific text relative to the corpus. It is therefore better at identifying themes, topics, and semantic emphasis.
The corpus contains eighteen Project Gutenberg texts by six writers: H.G. Wells, Philip K. Dick, Leigh Brackett, Andre Norton, Henry Kuttner, and Marion Zimmer Bradley. These authors span different decades, national moments, and subgenres. Some write planetary adventure, others invasion fiction, philosophical speculation, or postwar paranoia. Rather than asking only what these stories mean through close reading, this assignment asks a different question: what patterns emerge when machines compare them?
The answer is not that computers replace reading. Instead, they produce another kind of reading. As we discussed throughout the course, digital humanities tools allow us to detect structures too large or subtle to notice manually. At the same time, they require caution, interpretation, and awareness of limits. This essay argues that Stylo and TF-IDF reveal complementary truths: one maps authorial habit, the other maps thematic imagination.

## The Corpus as Historical Evidence
Before examining the visualizations, the corpus itself deserves attention. Although grouped under “science fiction,” these texts were not produced under one single historical condition. H.G. Wells belongs to the late nineteenth and early twentieth century, when science fiction often emerged from imperial expansion, industrial modernity, and Darwinian thought. The War of the Worlds and The Island of Doctor Moreau reflect anxieties about invasion, species boundaries, and civilization.
By contrast, writers such as Philip K. Dick, Andre Norton, Brackett, Bradley, and Kuttner mostly wrote during or after the Second World War and into the Cold War. Their worlds are shaped by nuclear fear, bureaucracy, mechanization, propaganda, militarism, and the possibility that technology might outgrow human control. Science fiction in the 1950s often became a disguised commentary on contemporary life.
This historical split matters because computational models often capture chronology indirectly. A writer from 1898 may appear distant not because of weaker literary quality, but because syntax, punctuation, and lexical preference differ across eras.

## What Stylo Measures: Writing Without Plot
Figure 1. Stylo hierarchical cluster analysis using 500 most frequent words.
Stylo was perhaps the most counterintuitive method used in this course. Human readers often focus on dramatic nouns and verbs: invasion, machine, planet, fear, death. Stylo instead pays attention to words many readers ignore. Yet those small words form patterns of rhythm and grammar that are difficult for writers to consciously disguise.
The 500 MFW cluster analysis shows several clear groupings. Philip K. Dick’s three texts remain close together. This suggests that despite different plots, Dick uses language in a stable and recognizable manner. Sentence construction, transitions, pronoun usage, or clause patterns may create a consistent fingerprint.
Andre Norton’s works also cluster tightly. This implies a steady narrative style, perhaps connected to direct prose, adventure pacing, and continuity of narration. Norton’s fiction often emphasizes movement and survival, and that consistency may extend into grammatical habits.
H.G. Wells appears relatively distant from many later writers. This is unsurprising. His prose belongs to an earlier literary period, and even common-word usage changes historically. Wells therefore becomes an outlier not simply because he is Wells, but because he writes from another linguistic moment.
The most unstable placement belongs to Henry Kuttner. His texts do not cluster as cleanly as Dick or Norton. There are several plausible explanations. Kuttner worked across multiple genres, including horror and fantasy, and stylistic range can weaken clustering. In addition, one corpus text was co-authored, which complicates stylometric identity by blending signals.
What Stylo reveals, then, is that genre membership does not erase individuality. Two authors can write science fiction while sounding structurally unlike one another.

## Why Parameter Choice Matters
One of the strongest lessons from this assignment is that digital results depend on settings. At lower MFW counts such as 100, some clusters were noisier and less convincing. At 500 MFW, authorial patterns became clearer. This supports Maciej Eder’s argument that sample size and feature selection matter deeply in authorship studies.
A careless reader might assume a dendrogram is objective truth. In reality, it is partly an artifact of methodological decisions: number of words selected, culling percentage, distance measure, and corpus cleaning. This reinforces a broader course theme from our discussions of Google Ngram and Bookworm: tools do not simply reveal patterns—they construct them through design choices.

## What TF-IDF Measures: Distinctive Worlds
Figure 2. TF-IDF PCA plot showing thematic proximity among texts.
If Stylo asks who writes alike, TF-IDF asks what kinds of worlds these texts talk about. By down-weighting common words and emphasizing distinctive vocabulary, it maps thematic similarity.
The PCA visualization shows several compelling relationships. Brackett and Bradley move nearer to one another than they do in Stylo. This likely reflects shared genre vocabulary associated with planetary romance, strange societies, conflict, travel, or exotic landscapes. Their sentence habits may differ, but their imaginative lexicons overlap.
Philip K. Dick remains somewhat coherent here as well. His fiction repeatedly circles war systems, defensive structures, paranoia, machinery, and unstable human identity. This suggests that Dick possesses both a stylistic signature and a thematic signature.
H.G. Wells again appears separate, but for different reasons than in Stylo. Here the separation likely emerges from vocabulary fields linked to evolution, invasion, vivisection, empire, or civilization. He is not merely stylistically older; he is lexically tied to earlier scientific concerns.
Andre Norton often occupies a space associated with travel, danger, exploration, and survival. Her works may cluster because of recurring adventure vocabulary rather than grammar.
TF-IDF therefore shows that science fiction contains multiple subgenres operating under one umbrella label. “Science fiction” is less a single mode than a coalition of narrative interests.

## Where the Methods Disagree
The richest interpretive moments occur when the two models disagree. If Brackett and Bradley are close in TF-IDF but not in Stylo, that suggests shared themes without shared voice. If Kuttner is unstable in Stylo but more coherent in TF-IDF, it suggests changing prose habits inside a relatively consistent thematic zone.
These disagreements matter because they challenge the simplistic claim that style and content are fully separable. In theory, one can measure grammar separately from vocabulary. In practice, literature blends them constantly. A paranoid theme may produce abrupt syntax. Expansive world-building may generate descriptive sentence forms. Adventure pacing may shorten clauses. Form and content influence one another.
This is why digital humanities works best when methods are compared rather than used alone.

## Reading the Cold War Through Data
This corpus also taught me something about the historical imagination of the 1950s. Even without close reading of every text, patterns suggest recurring postwar anxieties. Dick’s concentration around defense, systems, and control reflects fears of depersonalized institutions. Norton’s exploratory plots reflect mobility and frontier logic. Brackett and Bradley show continued attraction to off-world societies and alternate orders. Wells remains the ancestor whose earlier fears—species collapse, invasion, scientific arrogance—still echo later in the genre.
Science fiction thus becomes a record of changing modern fears. Computational analysis cannot feel those fears, but it can show their lexical repetition.

## Underwood and the Limits of Distant Reading
Ted Underwood’s The Risks of Distant Reading was especially relevant here. He warns that quantitative methods can create overconfidence. A cluster does not explain irony, emotion, symbolism, or reader experience. It cannot tell us whether a machine in Dick is tragic, comic, or sacred. It only tells us that related words recur.
That warning is essential. TF-IDF might highlight the word war, but it cannot know whether the text glorifies war or condemns it. Stylo can group two authors, but it cannot explain why their voices feel emotionally different.
Yet Underwood does not argue that distant reading is useless. Rather, he asks scholars to use it responsibly. That is the best framework for this assignment. These methods are powerful when paired with interpretation, historical context, and skepticism.

## New Literacies from the Course
This project also reflects the broader technical skills developed throughout the semester. GitHub Pages, Markdown, Posit Cloud, Voyant Tools, and static site publishing changed what literary work can look like. Scholarship is no longer only essays in Word documents. It can involve repositories, reproducible notebooks, visual argumentation, and public-facing websites.
That shift requires new literacies. Students must learn not only to interpret texts, but to understand datasets, code settings, interface assumptions, and visual rhetoric. Knowing how to read a dendrogram is now as valuable as knowing how to read a paragraph.

## Conclusion
Comparing Stylo and TF-IDF transformed my understanding of science fiction and of reading itself. I initially expected a relatively unified corpus because all texts belonged to the same genre. Instead, the corpus fragmented into multiple authorial and thematic communities.
Stylo demonstrated that authors leave stable fingerprints in ordinary language. Dick and Norton cluster strongly, Wells remains historically distant, and Kuttner resists easy categorization. TF-IDF showed that thematic alliances cut across author boundaries: Brackett and Bradley can share imaginative terrain even when they do not share style.
The most important lesson is that literature contains multiple layers of pattern. Some belong to the author, some to the genre, some to history, and some to chance. No single method captures all of them. But when methods are compared critically, they make hidden structures visible.
Computers do not read like humans. They do not experience wonder, dread, suspense, or beauty. But they can help humans notice forms of repetition, distance, and similarity that would otherwise remain invisible. Used carefully, computational reading does not diminish literature. It enlarges the ways we can encounter it.

READY FOR GRADING!

## Works Cited
Eder, Maciej. “Does Size Matter? Authorship Attribution, Small Samples, Big Problem.” Digital Scholarship in the Humanities, vol. 30, no. 2, 2015, pp. 167–82.

Herman, David, and Mike Kestemont. “Can Computers Read Literature?” Course reading.

Hermeneutica. Chapter 2, “How Computers Measure Words.” Course reading.

Underwood, Ted. Distant Horizons: Digital Evidence and Literary Change. University of Chicago Press, 2019.

Crymble, Adam. “Building the Invisible College.” Course PDF.
