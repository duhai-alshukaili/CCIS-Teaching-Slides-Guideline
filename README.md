# CCIS Guideline for Teaching Slide Decks

A common minimum standard for teaching slide decks used in College of Computing and Information Sciences (CCIS) courses across all UTAS branches, together with a background study and ready-to-use course templates for PowerPoint and LaTeX Beamer.

## Purpose

A teaching slide should help students think, not serve as the lecturer's script. This guideline gives CCIS faculty a shared, evidence-based standard for designing lecture decks so that:

- slides reduce unnecessary cognitive load and support learning;
- every course presents a consistent, professional look across branches;
- decks are accessible to all students, including those with color vision deficiency or who use screen readers;
- others' work is acknowledged and sources are cited, holding faculty to the same academic integrity standard expected of students;
- use of generative AI is disclosed and verified.

The recommendations draw on Cognitive Load Theory (Sweller), Mayer's Cognitive Theory of Multimedia Learning, the Assertion-Evidence framework (Alley and Garner), and WCAG 2.2 accessibility standards. Where the evidence is strong the guideline says "must"; where it is good practice or course-dependent it says "should" or "consider".

## Summary of the guideline

The guideline covers ten areas. Each gives a short rule followed by Good and Bad examples side by side.

| # | Area | Key points |
|---|---|---|
| 1 | Clear and simple design | One idea per slide. Prefer the Assertion-Evidence layout: a full-sentence headline stating the point, backed by visual evidence. Keep body text under about 40 words; move detail to speaker notes. |
| 2 | Proper use of graphics | Graphics must explain, not decorate. Place labels next to what they describe, use signaling to guide the eye, use vector or high-resolution images, and write alt text that states the point. |
| 3 | Font choice | One sans-serif family plus one monospaced code font. Headlines 32–40 pt, body 20–24 pt, nothing below 14 pt, code 18–22 pt. Sentence case, left-aligned. |
| 4 | University branding | Official UTAS logo (staff PNG) on the title slide. Do not use the corporate UTAS template for teaching; build one plain course template, agreed by the course team and used for every lecture at every branch. |
| 5 | Choice of colors | Restrained palette. Text contrast of at least 4.5:1 (aim for 7:1 in bright rooms). Never rely on color alone; pair it with shapes, line styles or labels. |
| 6 | Software tools | LaTeX Beamer, PowerPoint or Google Slides are all acceptable, but one course uses one tool and one template. Share as PDF on the LMS. |
| 7 | Information on the slides | Required title slide fields, measurable learning outcomes near the start, a summary, next steps and references at the end. No student personal data. |
| 8 | Attributing others' contributions | Acknowledge reused slides on the title or credits slide, respect publisher and Creative Commons terms, and disclose AI assistance. |
| 9 | Referencing and citations | Cite every borrowed figure, table, dataset or code sample on its slide (14 pt minimum) and in a full References slide. APA 7 recommended; IEEE allowed if used consistently across the course. |
| 10 | Sectioning and transitions | Three to five sections tied to the lecture outcomes, with divider slides, bridging questions, a check for understanding per section, and a recap. |

The guideline ends with a pre-upload checklist. Sections 4, 8 and 9 (branding, attribution and citations) are the priority when adapting existing decks, because they carry institutional and legal weight.

## Repository contents

```
Teaching Slides Guideline/
├── Guideline/
│   ├── CCIS Guideline for Teaching Slide Decks.docx   The guideline (editable)
│   ├── CCIS Guideline for Teaching Slide Decks.pdf    The guideline (for distribution)
│   └── Higher Education Slide Design.docx             Background study
└── Reference Template/
    ├── CCIS_Teaching_Template.potx                    PowerPoint course template
    └── CCIS_Teaching_Template-Beamer/                 LaTeX Beamer course template
        ├── beamerthemeCCIS.sty                        The CCIS Beamer theme
        ├── lecture-template.tex                       Sample lecture following the guideline skeleton
        ├── lecture-template.pdf                       Compiled sample
        ├── references.bib                             Sample APA 7 bibliography
        ├── utas-logo.png                              Official UTAS logo (do not modify)
        └── README.md                                  Build and usage notes for the theme
```

- **Guideline** – the *CCIS Guideline for Teaching Slide Decks* in Word and PDF form, and the background study *Pedagogical Slide Design in Higher Education: Cognitive Architecture, Visual Aesthetics, Academic Integrity, and Generative AI Integration*, on which the guideline's recommendations are based.
- **Reference Template** – two reference implementations of a course template that meets the guideline (title, section divider, content and closing layouts; slim footer; fixed fonts and palette). Course teams can adopt one as a starting point and adapt it for their course. See the Beamer [README](Reference%20Template/CCIS_Teaching_Template-Beamer/README.md) for build instructions and theme commands.

## AI acknowledgement

Generative AI tools were used in preparing this material:

- **Google Gemini** was used to synthesize the background study (*Higher Education Slide Design*) from the provided references.
- **Claude** (Anthropic) was used to draft the guideline based on the background study.
- **Claude Design** was used to create the course templates (PowerPoint and Beamer).

All content was reviewed and verified by the author, who remains responsible for it.
