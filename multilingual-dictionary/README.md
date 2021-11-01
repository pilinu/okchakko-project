# multilingual-dictionary
The aim of this project is to create a multilingual dictionary. The relevant languages are major languages and endangered languages. To begin with, we shall focus on the italian-gallurese, italian-sassarese, italian-logudorese, italian-campidanese, italian-sicilian pairs.

# File structure
For the sake of simplicity, the dictionary format will be .csv. Each language will have several dedicated columns:
- word: fre, ita, sdn for (respectively) french, italian and gallurese words
- grammatical type: freT, itaT, sdnT for (respectively) french, italian and gallurese grammatical types
- rule type: freR, itaR, sdnR for (respectively) french, italian and gallurese rule types: this item is used used to compute plurals of nouns or adjectives, as well as conjugated forms of verbs. 

# Grammatical typology
<img align="right" width="20%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/British_and_European_butterflies_and_moths_%28Macrolepidoptera%29_%28Plate_XII%29_%286466293519%29.jpg/600px-British_and_European_butterflies_and_moths_%28Macrolepidoptera%29_%28Plate_XII%29_%286466293519%29.jpg">

The multilingual dictionary will only contain lemmas (derived forms will be computed lately). The main grammatical types are:
- masculine singular common nouns : NCms
- feminine singular common nouns : NCfs
- masculine singular proper nouns: NPms
- feminine singular proper nouns: NPfs
- masculine singular adjectives : AQms
- infinitive verbs: INF
- adverbs: ADV
- prepositions: PS

# Multiple grammatical types
Some words have different grammatical types. For example, 'cardinale' in Italian (and 'cardinal' in French) can be both a common noun (NCms) and an adjective (AQms). This results in two entries in the multilingual dictionary:
- cardinale, NCms
- cardinale, AQms

# Language codes
The codes used to name each language are those from the iso 639-2 standard. These three-letter codes are included in the iso 639-2_codes file (see [List of ISO 639-2 codes](https://en.wikipedia.org/wiki/List_of_ISO_639-2_codes) and also https://www.loc.gov/standards/iso639-2/php/code_list.php). For example:
- ita: Italian language
- sdn: Gallurese language

# Derived dictionaries
From the multilingual dictionary, we will be in a position to compute:
- a monolingual dictionary for each language concerned
- a bilingual dictionary for each pair of languages concerned

# Primary target
Our primary target will be the italian-gallurese, italian-sassarese, italian-loudorese, italian-campidanese, italian-sicilian pairs and thus the associated translation.

## Gallurese language
- iso 639-2 code: sdn 
<img align="right" width="33%" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/10/Santa_Teresa_Gallura_-_Capo_Testa_%2818%29.JPG/512px-Santa_Teresa_Gallura_-_Capo_Testa_%2818%29.JPG">
The Gallurese language is one of the four languages (along with Sassarese, Logudorese and Campidanese) which belongs to the macro-language of Sardinia. The Gallurese language belongs to the Italo-Dalmatian family and is spoken in the region of Gallura, northeastern Sardinia. Gallurese morphology and vocabulary are close to southern Corsican, especially the 'sartinese' variant, whereas its phonology and syntax are similar to those of other Sardinian languages. One third of Gallurese vocabulary is also influenced by Logudorese Sardinian, Catalan, and Spanish (adapted from wikipedia article).

In a first step, we will implement one of the main variants of the Gallurese language (we will preferably choose a well documented variant, such as the one used in the writings of Maria Teresa Inzaina). Later on, the main variants of the Galluese language will have to be integrated. 

The mode of writing in Gallurese will be that which appears in the writings of Maria Teresa Inzaina:

- [Tizzoni](https://www.luigiladu.it/contos/tizzoni.htm), a short story of Maria Teresa Inzaina and Antonio Meloni
- [Li fiori di l’alburi di la presca](http://www.accademiasarda.it/2014/12/li-fiori-di-lalburi-di-la-presca-di-maria-teresa-inzaina/), short story of Maria Teresa Inzaina
- [La fura](https://www.luigiladu.it/contos/la_fura.htm), short story of Maria Teresa Inzaina
- [Tummeantoni (l’ultimu carrulanti)](https://www.luigiladu.it/contos/tummeantoni.htm), short story of Maria Teresa Inzaina
    
## Sassarese language
- iso 639-2 code: sdc

## Logudorese language
- iso 639-2 code: src 

## Campidanese language
- iso 639-2 code: sro 

## Sicilian language
- iso 639-2 code: scn 

# Evolution
Lately, further columns will be added for each language:
- lemma: for derived words
- rule: how to generate plural or conjugated forms of verbs

