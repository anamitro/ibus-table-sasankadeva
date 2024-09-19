# Sasankadeva keyboard for Bengali script
<img src="Sasankadeva_bn.svg" alt="drawing" width="400"/>

## Motivations
Semi-phonetic, i.e., a midway between the accuracy of grammatical typing and the ease of phonetic Indic typing. The ease has been ensured in many ways, including spelling statistics, character combinations and multiple options to be used as suits. Along with our own set of input keys, most popular input strings from widely used Avro Phonetic and itrans-Bangla are also supported.

Unfortunately, awfully insufficient effort has been put by programmers from India to make a usable input engine for the Bengali script, especially for writers untrained in professional typing. Almost all the publishers, and even the catalogue-searching computers in the National Library, use alternatives from Bangladesh. Now, that's something I specifically wanted to change. Also, Bangladeshi keyboards that are run with inbuilt dictionaries for word suggestions, are inconvenient for the purer form of Indian Bengali, that has a substantially lesser extent of Arabic and Persian loan words that the language standardly spoken in Bangladesh.

Apart from useful well-defined shortcuts that save time while typing, we have fixed phonetic-based layout for all usual character combinations in Indian Bengali, so that the user can practically type without looking at the screen if he chooses to. Also, suggestions come up, to be selected from if one is more comfortable with them. We aim at making an algorithm that provides space for both well-defined inputs with phonetic variations, has sets of methods that suits both proffessional and layman typing with one or two hands, that are easy to learn and easier to apply. The interface has been built in ibus-table environment.

## Installation
- Dependency: ibus-table (generally installed by default)
- [GitHub repository](https://github.com/anamitro/ibus-table-sasankadeva/)
- Download the .deb file as per your requirements; we have a number of flexible options! Extract from the .zip file (if zipped) or simply save the .deb file in your preferred directory.
- Delete any previous version of Sasankadeva, if you already had it installed, and refresh ibus, e.g., in Ubuntu, by opening the terminal and then running:
  
    (a)    $ cd /usr/share/ibus-table/tables
  
    (b)    $ sudo rm ./Sasankadeva.db
  
    (c) Type Alt+F and then type 'r' without the quotes and Enter. Gnome desktop will refresh.
  
    (d) Log out and log back in.
  
- Open Settings > Languages and Region > Add input method (+).
  
    (a) If Bengali is your default language of OS, select বাংলা (ভারত) and select Bangla (শশাঙ্কদেব) from there.
  
    (b) Otherwise, the options for Bangla will be available among 'Others' (⋮). Select Bangla(Sasankadeva) from there.
  
- Optionally, Select Bangla (শশাঙ্কদেব) from input methods in Settings (or Ibus Preferences, by running ibus-setup in terminal).

## Typing Manual

### Vowels

|  |  |  |  |
| --- | --- | --- | --- |
| অ | আ | ই | ঈ |
| উ | ঊ | ঋ | ৠ |
| ঌ | ৡ | এ | ঐ |
| ও | ঔ |  |  |

| একক | স্বরবর্ণ |  |  |
| --- | --- | --- | --- |
| A | AA/aa | I | II |
| U | UU | R | R< |
| LLi | LLi} | E | AI |
| O | AU |  |  |

| স্বরবর্ণ | -কার |  |  |
| --- | --- | --- | --- |
|  | a | i | ii |
| u | uu | < | << |
| } | }} | e | ai |
| o | au |  |  |

### Consonants

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| ক | খ | গ | ঘ | ঙ |
| চ | ছ | জ | ঝ | ঞ |
| ট | ঠ | ড | ঢ | ণ |
| ত | থ | দ | ধ | ন |
| প | ফ | ব | ভ | ম |
| য | র | ল | ব | শ |
| ষ | স | হ | ড় | ঢ় |
| য় | ৎ | ং | ঃ | ঁ |

#### সাধারণ ব্যঞ্জনবর্ণ অ-কারান্ত রূপ ও যুক্তাক্ষরের প্রথম বর্ণ

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| k | kh | g | gh | Ng |
| c | ch | j | jh | & |
| T | Th | D | Dh | N |
| t | th | d | dh | n |
| p | f | b | v/bh | m |
| z | r | l | b | S |
| Sh | s | h | q | Q |
| y | { | ` | H | ~ |

#### যুক্তাক্ষরের পরবর্তী বর্ণ

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| K | Kh | G | Gh |  |
| C | Ch | J | Jh |  |
| Z | Zh | X | Xh | [ |
| V | Vh | W | Wh | > |
| P | F | w | Bh | M |
| ] | / | L | w |  |
|  | \s |  |  |  |
|  |  |  |  |  |

All conjunct second components can also be typed as
> \ (consonant as first component)

#### যুক্তাক্ষরের প্রথম বর্ণ

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
|  |  |  |  | n |
|  |  |  |  | n |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  | । |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

### Assamese

| ৰ | ৱ |
| --- | --- |
| r (assamese version) | B |

### Sanskrit

| 𑁍 | ঽ | ৺ | ্ |
| --- | --- | --- | --- |
| # | hh | ^ | \ |

### Symbols

| 𑁍 | ₹ | $ | 🇮🇳 |
| --- | --- | --- | --- |
| # | $ | $$ | ## |

### Zero Width Non Joiner
 _ (underscore)
 
 **Use:**
 
 | r\z | r_\z |
 | --- | --- |
 | র্য | ‍র‍্য |
 | । z | r] |
 
### BEGINNERS' VERSION
Lastly, the manual in detail might seem a bit difficult to remember. But, after being used to this method (and even that does not require much practice) it is truly very easy and fast. And not at all so complicated as it seems. To start with, you may use the Beginners version if it helps.

For the Beginners version, on typing one consonant key, all the yuktaksharas possible with that key **EXCEPT য-ফলা (]), র-ফলা (/), ব-ফলা (w), রেফ্ ($$\mid$$ ; before second consonant)** will show up in the suggestion strip. Enable maximum number of suggestions in Ibus Table Preferences to benefit from that.

### NAVIGATION
#### Switching between English and Bangla:
To change keyboard to English (or default keyboard by direct input), press Super+Space or press Shift key (generally twice works). To return to Bengali, press Shift again.
#### Navigate between suggestions:
To navigate between suggestions, use Up Arrow Key and Down Arrow Key. To select suggestion, press Shift.
#### Navigate within text:
To finalize text unit, do the same as above (Shift or double-Shift), and navigate through typed text using Left and Right Arrow Keys only after that. Note, unlike Avro and similar methods, here SpaceBar does not denote termination of text unit, rather Backspace, Enter, Shift Space, more than one Shift-s or Tab do.

## Sasankadeva
Sasankadeva was a 7th century king of Gauda (Bengal) who is remembered for his consolidation of Bengal's statehood and political prominence.

<img src="coin.jpg" alt="drawing" width="400"/> **<<** Coins in circulation during Sasankadeva's time

## Author
[Anamitro Biswas](https://anamitro.github.io)

**Email:** anamitroappu@gmail.com

[**Homepage**](https://anamitro.github.io)

🇮🇳 Made in India

Copyright (C) 2021-2024 Anamitro Biswas
