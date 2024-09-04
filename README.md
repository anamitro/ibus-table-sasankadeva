# Sasankadeva keyboard for Bengali script
![logo](Sasankadeva_bn.svg)

## Motivations
Semi-phonetic, i.e., a midway between the accuracy of grammatical typing and the ease of phonetic Indic typing. The ease has been ensured in many ways, including spelling statistics, character combinations and multiple options to be used as suits. Along with our own set of input keys, most popular input strings from widely used Avro Phonetic and itrans-Bangla are also supported.

Unfortunately, awfully insufficient effort has been put by programmers from India to make a usable input engine for the Bengali script, especially for writers untrained in professional typing. Almost all the publishers, and even the catalogue-searching computers in the National Library, use alternatives from Bangladesh. Now, that's something I specifically wanted to change. Also, Bangladeshi keyboards that are run with inbuilt dictionaries for word suggestions, are inconvenient for the purer form of Indian Bengali, that has a substantially lesser extent of Arabic and Persian loan words that the language standardly spoken in Bangladesh.

Apart from useful well-defined shortcuts that save time while typing, we have fixed phonetic-based layout for all usual character combinations in Indian Bengali, so that the user can practically type without looking at the screen if he chooses to. Also, suggestions come up, to be selected from if one is more comfortable with them. We aim at making an algorithm that provides space for both well-defined inputs with phonetic variations, has sets of methods that suits both proffessional and layman typing with one or two hands, that are easy to learn and easier to apply. The interface has been built in ibus-table environment.

## Installation
- Dependency: ibus-table (generally installed by default)
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
- 
### BEGINNERS' VERSION
Lastly, the manual in detail might seem a bit difficult to remember. But, after being used to this method (and even that does not require much practice) it is truly very easy and fast. And not at all so complicated as it seems. To start with, you may use the Beginners version if it helps.

For the Beginners version, on typing one consonant key, all the yuktaksharas possible with that key
            **EXCEPT য-ফলা (]), র-ফলা (/), ব-ফলা (w), রেফ্ (| ; before second consonant)**
will show up in the suggestion strip. Enable maximum number of suggestions in Ibus Table Preferences to benefit from that.

### NAVIGATION
#### Switching between English and Bangla:
To change keyboard to English (or default keyboard by direct input), press Super+Space or press Shift key (generally twice works). To return to Bengali, press Shift again.
#### Navigate between suggestions:
To navigate between suggestions, use Up Arrow Key and Down Arrow Key. To select suggestion, press Shift.
#### Navigate within text:
To finalize text unit, do the same as above (Shift or double-Shift), and navigate through typed text using Left and Right Arrow Keys only after that. Note, unlike Avro and similar methods, here SpaceBar does not denote termination of text unit, rather Backspace, Enter, Shift Space, more than one Shift-s or Tab do.

## Example
| narayN$^\$ nmsK narnCaib nrotVmm\. debii` srswtii` byas` tto jymudiirye{.. | নারায়ণং নমস্কৃত্য নরঞ্চৈব নরোত্তমম্। দেবীং সরস্বতীং ব্যাসং ততো জয়মুদীরয়েৎ॥ |
| --- | --- |

## Author
[Anamitro Biswas](https://anamitro.github.io)

**Email:** anamitroappu@gmail.com

🇮🇳 Made in India

Copyright (C) 2021-2024 Anamitro Biswas
