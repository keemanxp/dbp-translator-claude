# Malay Translator Skill for Claude (DBP Standard Malay)

**Author:** Chuah Kee Man (https://chuahkeeman.com | kmchuah@unimas.my)

A Claude skill that translates English text into standard Bahasa Melayu following [Dewan Bahasa dan Pustaka (DBP)](https://www.dbp.gov.my/) conventions.

## What It Does

- Translates English to Bahasa Melayu across all text types — formal documents, technical/academic content, creative & marketing copy, and everyday text
- Strictly uses **DBP standard Malay** (no Indonesian variants)
- Flags uncertain or novel terms with concise notes while still providing the best available translation
- Supports flexible output formats: inline translation, side-by-side (EN ↔ BM), or downloadable `.docx`
- Preserves source formatting, adapting structure where it reads more naturally in Malay

## Key Features

- **DBP compliance** — uses Malaysian forms (*kerana* not *karena*, *maklumat* not *informasi*, *hospital* not *rumah sakit*) and DBP-approved terminology
- **Register awareness** — adapts tone to match the source material, from formal *surat rasmi* phrasing to punchy marketing copy
- **Smart term handling** — flags terms without established DBP equivalents (e.g. newer tech jargon) with inline notes, so you always know where the translation is on solid ground and where it's best-effort
- **Natural fluency** — translates for meaning and readability, not word-for-word

## Installation

1. Download the repo or the `SKILL.md` file (right click and save as)
2. Add it to your Claude skills directory in your Claude account (e.g. `/mnt/skills/user/dbp-translator/SKILL.md`)

Or, if you have the packaged `.skill` file, install it directly in Claude.

## Usage

Once installed, the skill triggers automatically when you ask Claude to translate English to Malay. For example:

- *"Translate this to BM: [your text]"*
- *"Terjemah ke Bahasa Melayu: [your text]"*
- *"Tukar ke BM: [your text]"*

You can also request specific output formats:

- **Side-by-side:** *"Translate this to BM in a side-by-side format"*
- **Document:** *"Translate this to BM and give me a Word doc"*

## Example

**English:**
> The cloud-based platform enables seamless collaboration across distributed teams, leveraging AI-driven insights to boost productivity.

**Bahasa Melayu (DBP Standard):**
> Platform berasaskan pengkomputeran awan ini membolehkan kerjasama yang lancar dalam kalangan pasukan yang tersebar, dengan memanfaatkan cerapan dipacu kecerdasan buatan bagi meningkatkan produktiviti.

## Licence

This skill is shared freely. Use it, adapt it, improve it.
