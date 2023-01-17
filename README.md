# labbcat-doc

Documentation, course materials, etc. for LaBB-CAT

These are HTML documents that can be browsed directly here:  
https://nzilbb.github.io/labbcat-doc/

## Updating the documentation

The documentation is plain HTML, and can be updated directly with your favourite text
editator. 

However, it was authored using a WYSIWYG HTML editor, which you can also use for updating
the documents. The editor is called
[wysiwiki](https://github.com/robertfromont/wysiwiki)
and is included in this repository for you convenience. To us it, you need to have Java
installed on your system.

To edit a particular set of documentation, you need to run a shell in the subdirectory of
the documents you want to edit, and run `java -jar wysiwiki.jar`.

This will open a browser window showing the files, and you can click the *Edit Page* button in
the top right corner to edit the document directly in your browser. Once you've finished,
click the *Save Page* button in the top right corner to save your changes.

e.g. to edit the *course* documentation:

```
cd course
java -jar wysiwiki.jar
```