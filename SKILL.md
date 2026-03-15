---
name: dbp-translator
metadata:
  author: Chuah Kee Man
description: >
  Translate English text into standard Bahasa Melayu following Dewan Bahasa dan Pustaka (DBP) conventions.
  Use this skill whenever the user asks to translate English to Malay, Bahasa Melayu, or BM — including
  formal documents, technical/academic content, creative writing, marketing copy, and everyday text.
  Also trigger when the user pastes English text and asks for a Malay version, says "translate this to BM",
  "terjemah", "tukar ke Bahasa Melayu", or any similar phrasing. This skill applies even for short phrases
  or single sentences — any English-to-Malay translation request should use it.
---

# English to Bahasa Melayu Translator (DBP Standard)

Translate English text into standard Bahasa Melayu that adheres to Dewan Bahasa dan Pustaka (DBP) conventions. The goal is fluent, natural-sounding Malay that a DBP editor would approve of — not stiff word-for-word substitution.

## Core Principles

### 1. DBP Standard Malay Only

Always use standard Malaysian Malay as recognised by DBP. This means:

- Use Malaysian forms, never Indonesian variants. Common examples:
  - *kerana* (not *karena*), *bahagian* (not *bagian*), *mesyuarat* (not *rapat*)
  - *maklumat* (not *informasi*), *perisian* (not *perangkat lunak*)
  - *kakitangan* (not *karyawan*), *mengesyorkan* (not *merekomendasikan*)
  - *hospital* (not *rumah sakit*), *kerajaan* (not *pemerintah*)
- Follow standard DBP spelling conventions (Sistem Ejaan Rumi Baharu) for general compliance — e.g. *syor* not *sor*, *kaji selidik* not *kajiselidik*.
- Use DBP-approved terminology where it exists. When translating technical, scientific, or specialised terms, prefer the term found in Kamus Dewan or DBP's terminology databases (e.g. PRPM — Pusat Rujukan Persuratan Melayu).

### 2. Natural, Fluent Translation

Translate for meaning and readability, not word-for-word. Good translation sounds like it was originally written in Malay.

- Restructure sentences where the English word order would sound awkward in Malay.
- Use appropriate Malay discourse markers and connectors (*walau bagaimanapun*, *selain itu*, *justeru*, *namun begitu*).
- Match the register of the source text — formal documents should sound formal in Malay; casual text should sound natural without being sloppy.
- For creative or marketing copy, prioritise impact and tone over literal accuracy. Adapt idioms and cultural references where a direct translation would fall flat.

### 3. Handling Uncertain or Novel Terms

Some terms — particularly in technology, pop culture, or very recent coinages — may not have an established DBP equivalent. When this happens:

- Still provide a translation using the best available Malay term or a reasonable calque/adaptation.
- Add a note in square brackets after the term, e.g.:
  > *pengkomputeran awan* [Nota: istilah DBP untuk "cloud computing"; penggunaan ini sudah diterima pakai]
- For genuinely novel terms with no clear DBP equivalent, note this explicitly:
  > *tokenisasi* [Nota: tiada padanan rasmi DBP setakat ini; "tokenisasi" digunakan secara meluas dalam bidang ini]
- Keep notes concise. They are there to flag uncertainty, not to provide a full linguistic essay.

### 4. Formatting and Structure

- Preserve the overall structure of the source text — headings, paragraphs, bullet points, numbered lists.
- However, feel free to adapt structure where it reads more naturally in Malay. For instance, an English sentence split across two bullet points might work better as a single flowing sentence in Malay, or vice versa.
- Maintain any emphasis (bold, italics) from the source.
- Do not translate proper nouns, brand names, or acronyms unless there is an established Malay equivalent (e.g. *PBB* for *UN*, *AS* for *US*).

## Output Format

The user may request different output formats. Default to **inline translation** unless they ask otherwise.

### Option 1: Inline Translation (default)
Simply provide the translated text. If there are flagged terms, the notes appear inline within the translation.

### Option 2: Side-by-Side
Present the English source and Malay translation in parallel — either as a two-column table or alternating paragraphs clearly labelled **EN** and **BM**.

### Option 3: Downloadable Document
If the user requests a file, create a .docx document containing the translation. For side-by-side documents, use a two-column table layout. Read the docx skill at `/mnt/skills/public/docx/SKILL.md` before creating any Word documents.

When the user doesn't specify a format, use inline translation and keep things clean and readable.

## Register Guide

Adapt your Malay register to match the source material:

- **Formal/official documents**: Use full formal Malay. Avoid contractions or colloquialisms. Employ *bahasa istana* conventions where appropriate (e.g. formal surat rasmi phrasing).
- **Technical/academic**: Use precise DBP-approved terminology. Maintain academic tone. It's fine to keep internationally recognised technical terms in their original form if no DBP term exists, but flag them.
- **Creative/marketing copy**: Prioritise tone, rhythm, and persuasive impact. Adapt freely — the translation should *feel* right, not just be technically correct. Malay wordplay or cultural resonance is encouraged where it fits.
- **General/everyday text**: Natural, conversational standard Malay. Readable and clear without being overly stiff.

## Common Pitfalls to Avoid

- **False friends with Indonesian**: Be vigilant. Words like *polisi* (Indonesian for "police") vs *polis* (Malaysian), or *bisa* (Indonesian "can") vs *boleh* (Malaysian) are easy traps.
- **Over-borrowing English**: Resist the temptation to keep English words when a perfectly good Malay equivalent exists. Use *tetingkap* not *window* (in computing), *muat turun* not *download*, *kata laluan* not *password*.
- **Passive voice overuse**: English formal writing often uses passive voice. Malay handles this differently — don't mechanically convert every English passive into a *di-* construction if an active sentence reads better.
- **Literal idiom translation**: "Break a leg" is not *patahkan kaki*. Find a Malay equivalent or convey the intended meaning naturally.

## Example

**English source:**
> The cloud-based platform enables seamless collaboration across distributed teams, leveraging AI-driven insights to boost productivity.

**Malay translation (inline with notes):**
> Platform berasaskan pengkomputeran awan ini membolehkan kerjasama yang lancar dalam kalangan pasukan yang tersebar, dengan memanfaatkan cerapan dipacu kecerdasan buatan bagi meningkatkan produktiviti.

This reads naturally in Malay, uses DBP-compliant terms (*pengkomputeran awan*, *kecerdasan buatan*, *cerapan*), and restructures the sentence for Malay flow rather than mirroring English syntax.
