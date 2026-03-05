---
title: Note-taking Conventions - N3RDIUM's Notes
description: WIP
template: n3rdium.dev
---
[TOC]
# Context
This vault is going to be used with a static site generator in order to cleanly integrate this with my website. Every time this repository is committed to, a webhook will trigger pages deploy on `n3rdium.dev`. That’s what I plan to do around April 2026.

Avoid renaming, since URLs need stability. For some amount of safety netting, you can implement a redirect system (markdown syntax with a redirect property). This is to be avoided as well, since it ruins UX.

The structure plan will keep this in mind, along with longevity. I really need this structure to *just work,* with minimal refactoring. For decades to come. That’s going to be a fun challenge to tackle.

Remember that *you’re not writing a textbook here.* These are *highly optimized, distilled notes.* Structure them appropriately. It’ll be completely useless if this ends up turning into a textbook.
# Paths
All file and folder names will be `lowercase with spaces`. Unless they’re universally accepted and dominantly used in literature, the use of abbreviations is to be avoided. This will make way for readable URL slugs and cool stuff like that.
# Levels
Separate knowledge into *levels,* like:

* #intro
* #ug
* etc.
# Subjects
Currently “registered” subjects:

* #physics 
* #chemistry
* #math
* #cs
# Structure
## concepts/
Individual notes in these directories will contain the notes for a specific topic in said subject. If multiple notes overlap too much, *merge them. No exceptions.* Each note will address only ONE topic or concept.
## courses/(level)
Notes will contain structures and links to all other data types (concepts, derivations, problems, doubts, etc.) in a course-curriculum-like structure. No actual text material, just structure.
## problems
Selected, interesting problems. No redundancy. Explore at most one each of a variety of problems instead of compiling those boring “problem sets”. This part of the vault is currently considered to have a relatively low priority.
## derivations/
Keep derivations separate from concepts, linking between them instead. This allows for a much more streamlined structure.
## doubts/
An index of doubts I’ve asked, along with answers and links to the concepts/derivations that helped resolve the doubt. Each file will have a `status` property which can hold one of three values: {open, resolved, obsolete}. Doubts need not start from the `inbox/` directory.
## projects/
This section of the vault is currently highly experimental. I intend to add *practical* stuff to complement the theory.
## research/(title)
Either individual notes, or non-recursive directories. This area is also highly experimental.
# Notes
Each file has a `subjects` property wherever applicable. Subjects is plural because the text may span across multiple subjects.

Wherever applicable (especially if it’s in the vault already), each note is to have a “prerequisites” section/tags.
# Disambiguation
When two notes from different subjects containing different concepts clash names, a “disambiguation” page with that name is to be created, which links to separate pages specific to these subjects, concatenated with `<subject>_`.
# Footnotes
Use footnotes generously to:

- Mark or link to sources, especially if they’re external
- Explain edge cases, caveats, gotchas, etc. without breaking flow
# Inbox
Almost all notes in this vault are born in the `inbox/` directory. Ideas start here, and get refined.

Notes in the `inbox/` directory *must* stay orphaned. Intended links will be denoted `[[like this]]` until “the orphan gets adopted” and makes its way into “the structure”.

Use `#todo` tags to mark sections of an orphan that need work. An orphan cannot be adopted unless all `#todo` tags have been resolved.
# Updates
Each file (or heading or list entry, if applicable) will contain these `#<level>` tags. This will improve accessibility. Whenever a topic is learnt in more depth than before, the same note is to be appended to with relevant tags in place.
# Commits
All commits must state their purpose.

- `[meta]` if updating any meta files (this file, `readme`, etc.)
- `[inbox]` if adding new entries to the inbox
- `[refactor]` if refactoring, or transferring from the inbox to the actual structure.
- `[doubts]`
- `[concepts]`
- `[courses]`
- `[projects]`
- `[research]`
- `[rename]` or `[breaking]`
