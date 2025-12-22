I’m going to be using this vault with a custom webpage builder in order to cleanly integrate this with my website. Every time this repository is committed to, a webhook will trigger build and pages deploy on `n3rdium.dev`. That’s what I plan to do around April 2026.

All file and folder names will be `snake_case`. Unless universally accepted and dominate literature, the use of abbreviations is to be avoided.

Avoid renaming, since URLs need stability. For some amount of safety netting, you can implement a redirect system (markdown syntax with a redirect property). This is to be avoided as well, since it ruins ux.

The structure plan will keep this in mind, along with longevity. I really need this structure to *just work,* with minimal refactoring. For decades to come. That’s going to be a fun challenge to tackle.

I must remember that *I’m not writing a textbook here.* These are *notes.* Structure them appropriately. It’ll be completely useless if I end up writing a textbook. Each note will address only ONE topic or concept.

I also need to decide at this stage whether I’m going to keep things separate (grade 11 is clearly separable from, say, grade 12), or something like that. Ideally, I’d like to “freeze” what I’ve learnt, and link to “patches” later as my knowledge on the subject grows.

I’m facing this weird dilemma: I can keep things accessible to users by keeping the “levels” separate, but modifying the same notes over is a more elegant thing to do.

I guess that certain topics are taught in different years, so they should be easy to handle. The ones that are not, however, I will have to “patch” instead.

Or better, instead of patching files, include formal levels as tags under every file. Links must stay concise. Inbox notes *must* stay orphaned, no links to and from them at all. Things that are intended to be links may be denoted with `[this]` syntax, and later converted into `[[]]`.

Footnotes are neat. Use them, especially to mark sources.

If multiple notes overlap too much, *merge them. No exceptions.*

Now for the actual organization. The meta stuff (like naming conventions, this file, the `readme` and `todo`) go in the root directory. An `inbox/` folder will contain fresh notes that are ready for organization into my structure. I’ll have to run through my `inbox/` folder every once in a while.

Apart from that, there will be the following folders:
- `concepts/{p,c,m}` 
- `courses/{11,12,ug,m,phd}` files with links to concepts, (problems?), derivations, doubts, projects, research, etc. No text material, just structure and links to said notes.
- `problems/{p,c,m}` (or maybe not?) (only selected, interesting problems)
- `derivations/{p,c,m}` (or maybe not the {p,c,m} part if it isn’t necessary) keep these separate from the concepts link here instead.
- `doubts/{p,c,m}` index of doubts I have asked, along with answers (+links to the concept notes that answered it) (if they exist). Each file will have a property called “status”, which can hold one of three values {open, obsolete, resolved}.
- `projects/{p,c,m}`
- `research/`

Or instead of {11,12,ug,m,phd}, try:
- introductory
- undergraduate
- graduate
- phd

Commit messages will follow the below convention:
- `[meta]` if updating any meta files
- `[inbox]` if adding new entries to the inbox
- `[refactor]` if refactoring, or transferring from the inbox to the actual structure.
- `[doubts]`
- `[concepts]`
- `[courses]`
- `[projects]`
- `[research]`
- `[rename]` or `[breaking]`