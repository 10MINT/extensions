This extension provides some useful tools for the TinyDB component

## Functions
* void BackupTags
  * Stores all your tags and values in a json file
* void LoadBackupFile(`String file`)
  * Reads the file and adds all tags and values to the database
* void AppendToTag (`String tag`, `String object`)
  * Appends something to a tag. Behaviour depends on what is stored in `tag`
    * Appends items to a list, if the stored value is a list
    * Appends characters to a string, if the stored value is a string
    * Increments the tag by `object` amount if the stored value is a number
* void RemoveFromTag (`String tag`, `Object object`)
  * Removes something from a tag. Behaviour depends on what is stored in `tag`
    * Removes items from a list, if the stored value is a list
    * Removess characters from a string, if the stored value is a string
    * Decrements the tag by `object` amount if the stored value is a number

## Properties
* String FileName
  * Gets/Sets the name of the generated json file
* boolean ShowErrors
  * gets/sets whether to show errors or not

## Events
* FileSaved (`String fileName`)
  * Event indicating that the database has been written to `fileName`
* void BackupSuccessful()
  * Event indicating that the tags of the backup file have been added to the database

---

Current version number is 2

[Visit this topic](https://community.thunkable.com/t/free-tinydbtools-extension/24781) at [Thunkable](http:/thunkable.com) for updates.
