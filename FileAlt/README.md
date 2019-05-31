This extension provides additional methods to the File component.

(Before anyone starts complaining: I know that it still contains the File component's methods, but this extension was originally designed for my TextMe project and I don't want to drag a new component into the designer just for this few methods.)

## Methods
* void CopyFile (String sourceFileName, String destinationFileName)
  * Copies the content of `sourceFileName` to `destinationFileName`

## Properties
* String PathToAssets
  * returns the path to the assets folder (accessible with //)
* PathToData
  * returns the path to the data folder (accessible without any slashed before the file name)
* GetUri (String file)
  * returns the uri of `file` (starting with file://)
* AreFilesEqual (String file1, String file2)
  * compares `file1` and `file2` by content

## Events
* AfterFileCopied (String filename)
  * Event raised after the content has been copied successfully. `filename` corresponds to the destination file name of the `CopyFile` method

---

Current version number is 4

[Visit this topic](https://community.thunkable.com/t/testers-needed-for-filealt-extension/16277) at [Thunkable](http:/thunkable.com) for updates.