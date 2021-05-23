# ibus-table-bengali
(See the attached pdf file for better understanding)
DOCUMENTATION: Sasankadeva Unicode, a free add-on for typing Bangla in Linux
Copyright © 2021 Anamitro Biswas


1. (a) Requirements: 'ibus-table' must be installed in your computer and 'ibus' selected as the input method.
(b) To install ibus-table-Sasankadeva version 1.0, extract the .zip file or save the Sasankadeva.txt and Sasankadeva.svg in folder, such that these two files remain in a directory, say /<dir.>. Copy the .txt file in same directory with template.txt in ibus-table folder, and the icon with  ibus-table/icons. Refresh ibus. You'll be able to select Bangla (শশাঙ্কদেব) from Bengali input methods (Settings in Ubuntu 20.04, or ibus-setup).
	E.g., for Ubuntu, open terminal and run
	$ ibus-table-createdb -n /usr/share/ibus-table/tables/Sasankadeva.db -s /<dir.>/Sasankadeva.txt
	$ sudo cp /<dir.>/Sasankadeva.svg /usr/share/ibus-table/icons/
	$ ibus-daemon -drx

2. 'Sasankadeva (Unicode)' is semi-phonetic, i.e., a midway between the accuracy of grammatical typing and the ease of phonetic Indic typing. The ease has been ensured in many ways, including spelling statistics, character combinations and multiple options to be used as suits. Along with our own set of input keys, most popular input strings from widely used Avro Phonetic and itrans-Bangla are also supported.
	Apart from useful well-defined shortcuts that save time while typing, we have fixed phonetic-based layout for all usual character combinations in Indian Bengali, so that the user can practically type without looking at the screen if he chooses to. Also, suggestions come up, to be selected from if one is more comfortable with them. We aim at making an algorithm that provides space for both well-defined inputs with phonetic variations, has sets of methods that suits both proffessional and layman typing with one or two hands, that are easy to learn and easier to apply.

3. Basic Consonants:
	ক	খ	গ	ঘ	ঙ
	k	kh	g	gh	Ng
	চ	ছ	জ	ঝ	ঞ
	c	ch	j	jh	&
	ট	ঠ	ড	ঢ	ণ
	T	Th	D	Dh	N
	ত	থ	দ	ধ	ন
	t	th	d	dh	n
	প	ফ	ব	ভ	ম
	p	ph	b	bh	m
	য	র	ল	ব	শ
	Y	r	l		S
	ষ	স	হ	ড়	ঢ়
	Sh	s	h	q	Q
	য়	ৎ	ং	ঃ	ঁ
	y	t``	`	H	~
	ক্ষ
	x
	
4. Popular keys from Avro:
z for য
^ for ঁ
f for ফ
v for ভ
NG for ঞ

5. Mechanical rule for yuktakshara:
A consonant by default comes with an implicit অ-vowel attached. Other vowels are to be typed after that in formats described in place. However, for compund characters (yuktakshara), the general rule is something like this:
For ন্দ,
type 'n' for 'ন', followed by a '\' for virama or hasanta (্), and then type the second consonant 'd' for 'দ'
For compund characters with 3 letters, e.g., ক্ষ্ম,
type 'k', then '\', then 'Sh', then 'm'

6. Virama:
Like Avro, ',,' also gives a virama.

7. Uppercase rule for compound characters:
There is another shortcut for compund characters. Generally, if you type the second (also third) letter of the compound in uppercase the two letters are automaticallly joined without the virama, e.g., শ্চ can also be written as 'SC' instead of 'S\c'. For ঙ্খ type 'NgKh'.

Exceptions: Some letters don't follow this uppercase rule, viz., ট, ঠ, ড, ঢ, ত, থ, দ, ধ, ন, র, য, শ, ষ, স. Their codes for second letter in compounds are:
 ট	ঠ	ড	ঢ	ত	থ	দ	ধ	ন	র	য	ব
 Z	Zh	X	Xh	V	Vh	W	Wh	>	_	]	w
 									/
 
Obviously every compound character can be typed with the virama rule.
 
8. Some very much used suffixes:
 ব-ফলা:w
 য-ফলা:	]
 র-ফলা:	_ or /

9. Independent vowels:
	অ	আ	ই	ঈ
	A	AA	I	II
	উ	ঊ	ঋ	ঌ
	U	UU	R	LLi
	এ	ঐ	ও	ঔ
	E	AI	O	AU

10. Dependent vowels:
	অ	আ	ই	ঈ
		a	i	ii
	উ	ঊ	ঋ	ঌ
	u	uu	<		
	এ	ঐ	ও	ঔ
	e	ai	o	au

11. Popular input strings from Avro:
Otherwise dependent vowels carry the simple layout as itrans. Some popular alternatives from Avro:
ঋ(ৃ) rri
ঈ(ী) ee	

12. Deafault customizations:
To accelerate phonetic typing, the following customizations, have been made by default:
(a) vowels typed as dependent are automatically input as independent vowels at the beginning of a word, and sometimes case-specifically -at the end or middle of it, e.g., 'dao' automatically transliterates to 'দাও', as  is 'daO'. Generally, vowel after another vowel is independent.
(b) 'e' after a vowel takes 'য়ে’ form, as many verbs in Bangla end with. To type, say, 'নৌকাএ', as rarely seen in archaic Bangla, use 'naukaE'.
(c) To ease the process of writing compound characters, several phonetic shortcuts have been created, e.g.,
'nj' gives 'ঞ্জ'
'nk' gives 'ঙ্ক'
'ng' gives 'ঙ্গ'
'ngh' gives 'ঙ্ঘ'
'j>' gives 'জ্ঞ'; this one also from 'j\&'
etc.
(d) You'll probably become familiar and comfortable with all customizations in course of use.

9. Consecutive consonants or vowels:
To make a compromise between grammatical and phonetic systems of input, it might be that sometimes expected character combinations don't come from typed codes, e.g, to type 'কহিলেন', presumed code should be 'khilen' but in place of 'কহ', 'kh' gives 'খ' by default.
This happens rarely. Users are suggested to type the last letter in the problematic combination again (whenever this happens) in the same string, because in most feasible cases these anomalities have been fixed in such a way.
'khh' should give 'কহ'
As in 'দিই', 'dii' gives 'দী' but 'diii' gives 'দিই'

10. Punctuations:
The end of sentence in prose Bengali is Danda or '।' as you are already perhaps familiar with. Single fullstop yields '।', while double gives the double danda. Three consecutive dots give ellipsis. Comma, hyphen etc. are as usual, except that single slash gives র-ফলা and double slash gives slash (/).

11. Additionals for Sanskrit:
Though I have never come across the use of the ones other than Avagraha.

HH	ঽ
<<	ৄ
R<	ৠ
LLi}	ৡ
}	ৢ
}}	ৣ

I add to this list the symbol of Indian Rupee, dervied from the Devanagari script:

'$' gives '₹'
'$$' gives '$'

10. Navigate between suggestions:
To navigate between suggestions, use Up Arrow Key and Down Arrow Key. To select suggestion, press Shift.

11. Navigate within text:
To finalize text unit, do the same as above (Shift or double-Shift), and navigate through typed text using Left and Right Arrow Keys only after that. Note, unlike Avro and similar methods, here SpaceBar does not denote termination of text unit, rather Backspace, Enter, Shift Space, more than one Shift-s or Tab do.

12. Switching between English and Bangla:
To change keyboard to English (or default keyboard by direct input), press Shift Space or press Shift key (generally twice works). To return to Bengali, press Shift again.

Example. Here I type an example with input and output. Since, though customized more according to character-usage in Bengali the keyboard can also be used to type Sanskrit in Bengali script (as is common in large parts of India), what's more appropriate than:
নারায়ণং নমস্কৃত্য নরঞ্চৈব নরোত্তমম্।	narayN` nmsK<V] nrncaib nrotvmm\.
দেবীং সরস্বতীং ব্যাসং ততো জয়মুদীরয়েৎ।।	debii` srswtii` byas` tto jymudiiryet``..

Obviously, other input can also yield the same result, e.g., 'দেবীং' as 'debee`' etc.

14. User-made customizations:
You can make your own custom input strings but editing or adding to between BEGIN_TABLE and END_TABLE lines of Sasankadeva.txt file, but I'd advise you not to try that if you are not well-versed in computer coding, and not extremely proficient in Bengali grammer. One problematic line has the potential to ruin for you the whole, or at least a considerable part of, input table.
	However, make sure not to change anything above BEGIN_TABLE, maybe apart from 'maximum number of input keys'.

	Lastly, since written in detail, all this might seem very difficult to remember. But, after being used to this method (and even that does not require much practice) it is truly very easy and fast. And not at all so complicated as it seems. And I have typed this documentation with 'Sasanka'. Play with it, and write Bengali. Thank me later ;)
