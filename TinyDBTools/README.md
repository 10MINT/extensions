This extension provides some useful tools for the TinyDB component

## Functions
* void BackupTags
  * Stores all your tags and values in a json file
* AppendToTag (String tag, String object)
  * Appends something to a tag. Behaviour depends on what is stored in `tag`
    * Appends items to a list, if the tag is a list
    * Appends characters to a string, if the tag is a string
    * Increments the tag by `object` amount

## Properties
* String FileName
  * Gets/Sets the name of the generated json file
* boolean ShowErrors
  * gets/sets whether to show errors or not

## Events
* FileSaved (String fileName)
  * Event indicating that the database has been written to `fileName`

Current version number is 1

[Visit this topic](https://community.thunkable.com/t/free-tinydbtools-extension/24781) at [Thunkable](http:/thunkable.com) for updates.
