# NOTES.md — teaching preferences and working notes

## Faz's Teaching Preferences
- Prefers dense, information-rich content — no fluff
- Wants my recommended answer alongside any question I ask him
- Prefers to explore multiple approaches and be grilled before committing to one
- Concise responses preferred
- Coming from strong clinical background + medical education leadership

## Working Notes
- **RCEMLearning authenticated** — fazeennasser@gmail.com. iMIS login via admin-ajax.php action=imis_login_submit
- RCEM website is JS-rendered but PDFs are direct-linked
- Web search tool currently broken (Firecrawl 400 errors) — using direct curl
- Notes platform at ~/mrcem is the primary content source
- Faz previously built and sold NeurallyMed (AI-powered PLAB prep platform) — understands exam prep mechanics at a deep level
- Previously led 500k+ user medical education platform (DailyRounds/Marrow) — not a novice learner

## Key Documents Downloaded
- MRCEM Primary Regulations & Information Pack (Nov 2023): `/tmp/MRCEM_Primary_Regs_Pack.pdf` — contains official blueprint
- MRCEM Exam Regulations 2025: `/tmp/MRCEM_Exam_Regulations_2025.pdf`
- MRCEM SBA Sample Questions: `/tmp/MRCEM_SBA_Samples.pdf` — shows question style/difficulty

## Official Blueprint (from Primary Regulations Pack)
- Anatomy: 60Q (33%) — Upper/lower limb, thorax, abdomen, head/neck, CNS, cranial nerves
- Physiology: 60Q (33%) — Cellular, resp, CVS, GI, renal, endocrine
- Pharmacology: 24Q (13%) — By system + immunological, anaesthesia
- Microbiology: 17Q (9%) — Principles, pathogen groups
- Pathology: 9Q (5%) — Inflammation, immune, infection, wound healing, haematology
- EBM: 10Q (6%) — Statistics, methodology, critical appraisal

## RCEMLearning Structure
- **MRCEM Primary Practice 1-5**: 5 modules × 12 questions = 60 practice SBAs
- **SBA Revise 1-5**: Clinical SBA practice (for SBA exam, not Primary)
- **Question Talk Through 1-3**: Walkthrough videos
- **Topic Hubs**: Pharmacology and poisoning content
- **No structured didactic lessons** on RCEMLearning for Primary basic sciences — just practice questions

## Lesson Design Conventions (created 21 Jun 2026)
- Blueprint-context box (blue) at top of each lesson with question weight
- Exam-pattern box (pink) for recalled question formats
- Harder SBAs: clinical vignettes, "all EXCEPT", mechanism-level, cross-category
- Detailed feedback: correct answer explanation + distractor analysis
- Shared CSS: `assets/style.css` + lesson-specific `<style>` block
