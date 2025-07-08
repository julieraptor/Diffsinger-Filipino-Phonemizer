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

# Usage

Follow this guide to learn how to use the Diffsinger Filipino Phonemizer.

## Words are pronounced how it is spelled.

The g2p doesn't account for unique pronunciations of words in other languages.
<p>
For example, English words will be pronounced syllabically instead of being pronounced with an accent.

| Word | Usual pronunciation (IPA/ARPA) | G2P separation | G2P Pron. (IPA) | G2P Pron. (Arpabet)
| ---  | --- | --- | --- | --- |
| BIRTHDAY | bɜːtdeɪ (B EH R T D E Y) | B I DX TH D A J | bɪrθdaɪ | B IY R TH D AY
| CONFIRMAR | kumpˈiɾma (K UW M P IY R M A)| K O N F I DX M A R | konfiɾmaɾ | K OW N F IY R M AA R

![image](https://github.com/user-attachments/assets/707682c9-0193-4776-b6a8-5f3c4a56c4f5)
*Example with G2P subsituted with LIEE's configuration using PixPrucer's Megamodel Version: v2.8 MM SH LN*

![image](https://github.com/user-attachments/assets/ce8c2032-230f-4589-9ff0-b72515fd413b)
*Example with G2P subsituted with Nishiren's Arpasing-based configuration*

### To get the desired spelling, you may have to write the word how it should be pronounced.
![image](https://github.com/user-attachments/assets/03ee3f4f-8717-4f0c-ad56-eeaf553d1085)

*Example with G2P subsituted with Nishiren's Arpasing-based configuration*


## Dipthongs
Dipthongs are not combined. They are separated into two characters.

**Examples:**
<br>
- aɪ [AY] -> [A J]
- oʊ [OU] -> [O U]

![image](https://github.com/user-attachments/assets/2dd56a02-1f9f-4c6d-8c7c-be0cab4f045c)

## Glottal stops
Glottal stops are inserted depending on certain conditions:
   - Before a vowel, if the word starts with a vowel.
   - Between two consecutive of the same vowel.
        - **Example:** AA -> [A Q A], UU -> [U Q U]
   - By adding ['] in between vowels
     - **Example:** AALIS -> [Q A Q A L I S], INIIBIG -> [Q I N I Q I B I H]
   - By adding ['] at the end of a word ending with a vowel.

![image](https://github.com/user-attachments/assets/18a1e305-b01d-4f47-8d33-b0d5fec20f19)

     
## [ll] becomes [L J]

Consistent with Filipino pronunciation, words containing the phoneme [ll] will be converted to [L J]. Most of these words come from Spanish.

### If you do not want the word to follow the Filipino pronunciation, substitute [l] for [y] when writing the word.
<br>
**Example:** amarillo -> [Q A M A R I L J O], amariyo -> [Q A M A R I J O]

![image](https://github.com/user-attachments/assets/0d2ad88b-7a35-4d6d-a47a-45264a19f774)
*Example with G2P subsituted with LIEE's configuration using PixPrucer's Megamodel Version: v2.8 MM SH LN*



## Omit glottal stop before a word starting with a vowel.

By default, words starting with a vowel begin with a glottal stop.
<br>
### If you do not want the glottal stop, simply drag the glottal stop phoneme all the way next to the following vowel.

![image](https://github.com/user-attachments/assets/5223e09d-a913-4dd5-bf61-dee43113dab7)
*Example with G2P subsituted with LIEE's configuration using PixPrucer's Megamodel Version: v2.8 MM SH LN*


# Disclaimer
- julieraptor holds no responsibility to any incidents, damage, or loss by the user from downloading or using the phonemizer.
- julieraptor holds no responsibility to any incidents, damage, or loss that occurs to any third party as a result of usage of the phonemizer.
- julieraptor isn't responsible for any legal issues created from the use of the phonemizer.

# 【CONTACT INFORMATION】
- **Site:** [website](https://julieraptor.carrd.co)
- **YouTube:** [chulie_chu](https://www.youtube.com/channel/UCaJ0Q7aEmNdZAME8zvxQICg)
- **Email:** [raptorjulie@gmail.com](mailto:raptorjulie@gmail.com)

