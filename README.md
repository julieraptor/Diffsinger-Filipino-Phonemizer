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

#### Dipthongs are separated by character

#### Glottal stops are inserted depending on certain conditions
    - If the word is pronounced with a glottal stop.
    - Before a vowel, if the word starts with a vowel.
    - By adding in in using ['] in between vowels or at the end of a word with a vowel

![image](https://github.com/user-attachments/assets/2da7e171-e470-4cb3-baa4-86a0fe83da10)
![image](https://github.com/user-attachments/assets/409ac355-4859-4b55-aaeb-43e40f561cd0)
![image](https://github.com/user-attachments/assets/7d82ba7a-d558-43ce-a88d-c7be897c0237)

