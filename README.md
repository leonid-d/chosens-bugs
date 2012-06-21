On Android 2.2-4.0, if option's value are in russian there is a bug with autosuggest and search.

Suggest works only if you enter space, and then delete it. Search results in suggest will update only then you delete s symbol, nothing is shown then you enter new ones.

Search only works if there is a space in option's value AND if there is a space in query. If one of this conditions is not meet, search will not work. But even if it works it works very strange — it will find all options that includes first word, but entered part of the second word is ingored.

How to reproduce:

"Адмирала На" -- will find Адмирала Макарова
"Адмирала Нахимова" -- will find Адмирала Макарова
"Адмирала" -- will find Абаканская
If you enter "Александра Сергеевича А" suggest will find all options with word "Александра", but search will only find "Александра Сергеевича" — the first option.