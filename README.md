# DiffsingerFilipinoPhonemizer
*A Tagalog/Filipino g2p phonemizer for OpenUTAU for Diffsinger*
 
## 【 Information 】 

The Diffsinger Tagalog/Filipino Phonemizer was developed to support standardized Tagalog (Filipino). 
Theoretically, it could support other languages in the Philippines (Ilokano, Cebuano, etc.) and other Malayo-Polynesian languages (like Indonesian) with similar pronunciation.

| Data | Information | 
| ---  | --- |
| Graphemes | 28 |
| Phonemes | 30 |
| Word Entries | 24765 |

## 【 Credits 】 

| Name | Role | 
| ---  | --- |
| julieraptor | Developer, model trainer |

Special thanks to Hammy (my partner) for Python tool development for dictionary separation.

The dictionary this phonemizer was trained on was sourced heavily from [CUNY Wikipron for Tagalog](https://github.com/CUNY-CL/wikipron/tree/master).

## 【 How To Use 】 

### Words are pronounced how it is written.

The language is generally pattern-based. Therefore, it will follow these rules:

#### Dipthongs
Dipthongs are separated into two characters.

**Examples:**
[AY] -> [A Y] ([A J] in the g2p)
[OU] -> [O U]

#### Glottal stops
Glottal stops are inserted depending on certain conditions
   - If the word is pronounced with a glottal stop.
   - Before a vowel, if the word starts with a vowel.
   - Between two consecutive of the same vowel.
   - By adding ['] in between vowels
   - By adding ['] at the end of a word ending with a vowel.

