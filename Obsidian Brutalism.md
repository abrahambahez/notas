# A brutalist approach to knowledge management in Obsidian

Hi all, a really old Obsidian user here (I've used this app since v0.5 or so). I'm a Product Manager in a small startup and also an Anthropology PhD student. My main use case is Knowledge Management, and I'd like to share my personal approach to it, which I call "Brutalist" since it's the closest word I've found to describe the gist of this mindset, particularly in [the web elaboration](https://brutalist-web.design/).

The Brutalist approach is an epistemic, ethic and aesthetic way of work with digital notes. I call it Brutalist because it feels and looks pretty rough, but at least to me has been sturdy enough to keep me using the same system 3 years without changes. The first two dimensions are expressed in a set of guiding principles inspired by multiple sources. The aesthetic dimension is more free, and I share my personal approach after the principles.

**Separation of concerns**

Notes are not tasks, nor agendas, projects, essays, books or papers. Each functional component of knowledge and management should be separated in a consistent way (different apps, vaults, directories, files or blocks). If I cannot extract each component programmatically then it needs refactoring.

Same principle applies to content versus presentation. I love (and do) editorial and web design, but at a note, draft and final writing levels I don't care about them. Once content is ready, I can pass it through multiple pipelines that may include advanced CSS or In Design to focus on craft a better visual experience.

**You are always wrong**

Some people use a popular metaphor to classify its notes: from seed to evergreen tree. My notes have always the same status #ToBeImproved, ergo, that tag are useless. I can't tell how many times I have delete a perfectly written, densely linked note because it is essentially naive or wrong. Think about an idea as *evergreen* falls in an epistemic trap: to think about truth as an inherent value of some fact, data or belief. Confusing *truth* with *reality* is a western bias with ancient roots, as an anthropologist I cannot accept it, because there are multiple, intriguing ways of knowing. Truth is a product made of a dense network of ideas, people, objects and history, framed inside an epistemic paradigm; changing the paradigm changes the values. It doesn't matter if your vault is only about western medicine, thinking in a constructivist fashion will release new ways of intelectual creativity.

**Elaboration first**

Brutalism is know to show the *raw materials* of the building. In Obsidian, the raw material is mainly text (although it can be a drawing, a picture or any little piece of communicating media) and relations, elaboration is about the content. Elaboration is the process of *thinking by writing*. One problem with outliners is that they seem to follow the *train of thought* pattern, forming a *serial thinking* in which each bullet is an independent idea that may be related with the former without expliciting its relation. Outlining is good as starting point but you shouldn't leave the note without writing one or more paragraphs that structures your idea using logical or narrative connections.

Elaborate before anything, before creating directories, tags, even links. If you elaborate first, links will *emerge* and force your prose to change towards a neverending quality refining loop.

**Thinking before linking**

There are plenty of frameworks to link better your notes. From MOCS to Compass to Mental Models. To make explicit *in the prose* what is the reason of the link is always better. A link may be relevant for many reasons: 

- x note *is an instance of* y
- x *is a subset of* y
- x *is a semantic dependency of* P (x is a part of proposition P; without x, P makes no sense)
- x *is isomorphic to* y (shares the same formal structure)
- x *is an analogy* of y
- etcetera

To create a complex and rich network of personal knowledge you only need two things: text and links. In fact, as Gordon Brander has shown [in its fantastic essay](https://subconscious.substack.com/p/all-you-need-is-links), links act as tags, folders, comments, outliners.

That's all. Only four principles can make the cognitive architecture: separate functions, have a constructivist mindset, use prose to think and make your links explicit. After this point, I think that the Brutalist approach can have many *flavors*, I mean methods, tactics, workarounds, etc. I'll show some practical hints that have been useful to me.

**Truth to materials**

As text is the *beton brut*, the raw material, I follow some rules in my vault.

1. I write in source mode always. Seen some example notes in the Discord made me care about the [content-markup ratio](https://www.woorank.com/en/blog/are-text-to-html-ratios-important); markdown is one of the lightest markup languages, and we have managed to make it look like code (as a pure functional-syntax writing) and in many cases is only to get *visual output* (yaml visualization fields, declarative output in dataview). I see the markup as an aesthetic value, so I care about how and when I put italics, code blocks and so on.
2. I limit the subset of markdown features to write notes. Again, inspired [by the specification of subtext](https://github.com/subconsciousnetwork/subtext) by Gordon Brander, I try to use as minimal markup elements as posible. For long content formats, I use pretty standard markdown (plus some pandoc syntax to automate references using citeproc)
3. I see performance as a feature. Minimize plugins force me to take the most critical or versatile offered and try to make de most of them. For example, the Shell Commands plugin can replace the Git related ones, also the advanced search or text refactor features. Using Vim can search and replace by regex and enable some advanced editing. I have created a theme merging some css snippets that were related to better visualize markup syntax and app and relevant (to me) UI structure. You can finding in themes as "Brutalism". I will work in it to get a better reusable version if anyone is interested.

**How to construct notes**

I follow the classic division of notes: fleeting, references, permanent and add the daily note as a different category from fleeting for reasons I'm about to explain. All notes are constructions, building representations of observable an conceivable realities.

- The reference note is constructed as a *dialogue*, contrary to the popular idea of *put it in your own words* I think we should treat others as valid voices in our own notes, not as hidden abstracted references. A reference is a book, an article, a personal interview, a memorized quote I heard in the market. Our brains are not silos and our voices are not only ours, we are part of a dense *semiosphere*. Deliberately impose our voice as a monologue is a trick to hide others and stress ourselves (another western bias: individualism), but that doesn't change the fact that their voices are still there. Use your own words *as having a conversation*.
- The fleeting note is constructed as an open experimental device that includes jottings, doodles, post-its, secret personal languages, mindmaps, recordings os sound landscapes, handmade cartographies, drawings, bodily experiences and practices that will turn into embodied knowledge. All of that constitutes a living personal archive that usually won't live in Obsidian, but informs the elaboration via descriptions, embedded media and references.
- The permanent note is constructed as I described above: through elaboration and explicit linking
- The daily notes is used as an advanced field journal. As you can see, I'm not particularly convinced of that individualist emphasis, so I prefer to replace *personal reflection journaling* by *reflexivity journaling*, that is, putting me inside the network of culture, people, social structures, material objects and ecological relations to better understanding my ideas, privileges, biases and beliefs. To do this I have a special syntax for daily notes. A daily note has 4 blocks: descriptions, dialogs/quotes, personal annotations and analytical annotations. Descriptions are single paragraphs, dialogs are surrounded by dashes, personal annotations are surrounded by parenthesis, analytical annotations are links. This allow me to run multiple analysis (some automated) to my daily notes to abstract/discover ideas and patterns that are not only mine, but product of my particular historical situation

I hope this helps some of you. If you read it all, thank you. I'll be glad to discuss anything, but I have to say sorry if I delay responses, school + work + family absorb most of my time and energy.
[[log ztk]]