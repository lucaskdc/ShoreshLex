# ShoreshLex

ShoreshLex is an experiment in **text-driven language learning**: instead of learning a language from generic course material, you learn it from the texts you actually want to read or watch, with the vocabulary prioritized by how often it appears.

The name combines *lex* (words) with *shoresh*, the Hebrew word for "root", reflecting the focus on reinforcing word roots over time.

> **Status:** early concept. No application code yet.

## Core ideas

1. **Learn from your own material.** You bring the texts, documents, articles, and links you are interested in. Keeping the source material personal is meant to keep motivation high, because every lesson is something you already wanted to read or watch.

2. **Frequency first.** From each text, the app extracts its vocabulary and ranks words by how often they occur, both within the document and across the user's whole library. The most-used words are learned first, so comprehension grows as early as possible.

3. **Roots over time.** Words are grouped by their root or lemma family (for example, a verb and its conjugations and derivatives). Learning a root reinforces every word built on it, and reviews are scheduled over time so that roots, not isolated word forms, are what stick.

4. **AI as a leverage, not a replacement.** AI is used to do the tedious work around the material: tokenizing and lemmatizing text, identifying roots, producing glosses and example sentences in context, generating exercises, and explaining grammar when the user asks. The user remains the one doing the learning.

## Planned features

- **Material intake:** paste text, upload a document, or add a link. Videos and articles are supported through their transcripts or extracted text.
- **Vocabulary extraction:** tokenize and lemmatize each source, then build a frequency list per text and across the library.
- **Priority queue:** a learning queue ordered by frequency, with words already known or ignored filtered out.
- **Root map:** a view of word families, showing which roots are being learned and how many derived forms each one unlocks.
- **Reinforcement reviews:** spaced repetition that revisits roots and their derived words, with review sessions built from the user's own sentences.
- **Contextual reading:** each word is shown with its source sentence and a gloss, so it is always learned in context.
- **Progress view:** coverage of each text (the share of its running words the user already knows) and how that coverage grows over time.

## Open questions

- Which languages to support first, and whether the root model should be language-specific or generic.
- Which AI models and providers to use for extraction, glossing, and exercise generation, and how to keep costs predictable.
- Where the data lives: local-first storage versus a hosted account.
- How to handle languages with rich morphology (such as Hebrew or Arabic) that need diacritic- or root-aware tokenization.

## Getting started

Nothing to run yet. Once the project has a stack, this section will describe installation and how to run it locally.

## Contributing

The project is at the idea stage. Feedback on the concept and on the open questions above is welcome.
