This extension allows localization in App Inventor. Upload a JSON-formatted file in your app and the strings will be set based on the user's locale. An example file can be found in [translations.json](translations.json)

[What is I18n?](https://en.wikipedia.org/wiki/Internationalization_and_localization)

## Properties
* String File
  * Sets/gets the name of the json file. Accepts all file locations
* String Default
  * Sets/gets he name of the translation to choose when the user's locale/language is not found in the file
* boolean UseLocale `since version 6`
  * Sets/gets whether to use the locale or only the system language
* String Localize (String tag)
  * localizes the string stored in the tag
* String GetISO3Language
  * returns the system language in ISO3 format
* String GetISO3Country
  * returns the locale's country in ISO3 format
* String GetLanguage
  * returns the system language in ISO 693-1 format

## Methods
* <s>void Initialize</s> `deprecated since version 3`
  * Reads the content of the file
* void ReadFrom (String string)
  * Reads translations directly from a string. Is faster, but more inconvenient. Not recommended for a lot translations

A big thanks to @ColinTree to provide the source code of his [SysLang extension](https://github.com/OpenSourceAIX/ColinTreeSysLang).

---

Current version number is 6

[Visit this topic](https://community.thunkable.com/t/localization-extension/7063) at [Thunkable](http:/thunkable.com) for updates.
