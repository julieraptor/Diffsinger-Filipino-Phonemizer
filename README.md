# DiffsingerFilipinoPhonemizer
*A Diffsinger Tagalog/Filipino g2p phonemizer for OpenUTAU*
 
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

# Phoneme Chart
| Phoneme | IPA | Arpabet | Notes
| ---  | --- | --- | --- | 
| A| a | AH |  |
| B| b | B |  |
| D| d | D |  |
| DX| ɾ | DX |Can be substituted for IPA [r] |
| DY| dʒ | JH |  |
| E| ɛ | EH |  |
| F| f | F |  |
| G| g | G |  |
| H| ɣ | G |Can be subsituted for IPA [g]. Appears when following a vowel, but not before a consonant. |
| HH| h | H | |
| I| i | IY |  |
| J| j | Y |  |
| K| k | K | Non-aspirated |
| L| l | L | Laminal denti-alveolar (NOT "dark L") |
| M| m | M | |
| N| n | N | |
| NG| ŋ | NG | |
| NY| ɲ | [N] [Y] | Represented as ñ. Use phonetic hints for IPA [n j] if not available
| O| o | OW | |
| P| p | P | Non-aspirated |
| Q| a | Q | Glottal stop |
| S| s | S | |
| SY| ʃ | SH |
| T| t | T | Non-aspirated |
| TH| θ | TH |
| TS| tʃ | CH |
| U| u | UW |
| V| v | V |
| W| w | W |
| Z| z | Z |

# Information

### The language is generally pattern-based. 

The g2p doesn't account for unique pronunciations of words in other languages.
<p>
For example, English words will be pronounced syllabically instead of being pronounced with an accent.

| Word | Usual pronunciation (IPA/ARPA) | G2P separation | G2P Pron. (IPA) | G2P Pron. (Arpabet)
| ---  | --- | --- | --- | --- |
| BIRTHDAY | bɜːtdeɪ (B EH R T D E Y) | B I DX TH D A J | bɪrθdaɪ | B IY R TH D AY
| CONFIRMAR | kumpˈiɾma (K UW M P IY R M A)| K O N F I DX M A R | konfiɾmaɾ | K OW N F IY R M AA R

### Dipthongs
Dipthongs are not combined. They are separated into two characters.

**Examples:**
<br>
- aɪ [AY] -> [A J]
- oʊ [OU] -> [O U]

### Glottal stops
Glottal stops are inserted depending on certain conditions:
   - Before a vowel, if the word starts with a vowel.
   - Between two consecutive of the same vowel.
        - **Example:** AA -> [A Q A], UU -> [U Q U]
   - By adding ['] in between vowels
     - **Example:** AALIS -> [Q A Q A L I S], INIIBIG -> [Q I N I Q I B I H]
   - By adding ['] at the end of a word ending with a vowel.

