<head>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+Bengali:wght@100..900&display=swap" rel="stylesheet">
</head>

# Sasankadeva keyboard for Bengali script
<img src="cat.png" alt="drawing" width="200"/><img src="er.png" alt="drawing" width="200"/><img src="bn-sasankadeva.png" alt="drawing" width="400"/>

- **Custom Phonetic Engine** It is a specialized Unicode Bengali input engine designed for the ibus-table framework, focusing on a custom phonetic layout that prioritizes ease of typing.
- **Unique Transcription Rules** The engine uses a unique set of transcription rules specifically tuned for the Bengali language, aiming to provide a more intuitive experience than standard layouts.
- **Fixed layout** so that the user can type practically without looking at the screen if he chooses to.
- **Minor conjunct-related grammatical corrections** inbuilt.
- **Minimized input key strings** for faster typing.
- **Open Source Accessibility** Developed by Anamitro Biswas, the project is hosted on GitHub to allow for community contributions and transparent development of Bengali digital tools.  
- **Platform Support** As an ibus based tool, it is primarily designed for Linux environments, enabling seamless Bengali input across various applications and terminal emulators.


## Installation
- **Dependency**: ibus-table
- [**GitHub repository**](https://github.com/anamitro/ibus-table-sasankadeva/)
- Delete any previous version of Sasankadeva, if you already had it installed, and refresh ibus, e.g., in Ubuntu, by opening the terminal and then running:
````
$ cd /usr/share/ibus-table/tables
$ sudo rm ./Sasankadeva.db
````
Refresh

### From source:
Save .txt and .svg (logo) files in some directory path <dir.>. Check the names, which may vary. In Terminal, run
````
$ ibus-table-createdb -n /usr/share/ibus-table/tables/Sasankadeva_bn.db -s /<dir.>/Sasankadeva_bn.txt
$ sudo cp /<dir.>/Sasankadeva_bn.svg /usr/share/ibus-table/icons/
$ ibus-daemon -drx
````

### From .deb or .rpm:
Download .deb file in directory <dir.>. Check the name (here, assume sasankadeva_bn.deb)
````
$ cd /<dir.>
$ sudo dpkg -i sasankadeva_bn.deb
````
Similarly for rpm.

### From .db:
Copy the .db file with root access to /usr/share/ibus-table/tables/ and the logo .svg to /usr/share/ibus-table/icons/.

## Typing Manual

### Vowels

|  |  |  |  |
| --- | --- | --- | --- |
| <span style="font-family: 'Noto Serif Bengali', serif;">অ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">আ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ই</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঈ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">উ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঊ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঋ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ৠ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">ঌ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ৡ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">এ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঐ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">ও</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঔ</span> |  |  |

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
| <span style="font-family: 'Noto Serif Bengali', serif;">ক</span> | <span style="font-family: 'Noto Serif Bengali', serif;">খ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">গ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঘ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঙ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">চ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ছ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">জ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঝ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঞ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">ট</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঠ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ড</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঢ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ণ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">ত</span> | <span style="font-family: 'Noto Serif Bengali', serif;">থ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">দ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ধ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ন</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">প</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ফ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ব</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ভ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ম</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">য</span> | <span style="font-family: 'Noto Serif Bengali', serif;">র</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ল</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ব</span> | <span style="font-family: 'Noto Serif Bengali', serif;">শ</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">ষ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">স</span> | <span style="font-family: 'Noto Serif Bengali', serif;">হ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ড়</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঢ়</span> |
| <span style="font-family: 'Noto Serif Bengali', serif;">য়</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ৎ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ং</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঃ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ঁ</span> |

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

| <span style="font-family: 'Noto Serif Bengali', serif;">ৰ</span> | <span style="font-family: 'Noto Serif Bengali', serif;">ৱ</span> |
| --- | --- |
| = | B |

### Sanskrit

| 𑁍 | ঽ | ৺ | ্ |
| --- | --- | --- | --- |
| # | hh | ^ | \ |

### Symbols

| ☸ | ₹ | $ | 🇮🇳 |
| --- | --- | --- | --- |
| @ | $ | $$ | ## |

### Zero Width Non Joiner
 _ (underscore)
 
 **Use:**
 
 | r\z | r_\z |
 | --- | --- |
 | <span style="font-family: 'Noto Serif Bengali', serif;">র্য</span> | <span style="font-family: 'Noto Serif Bengali', serif;">‍র‍্য</span> |
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

Copyright (C) 2021-2026 Anamitro Biswas
