# A module to parse .bib file to DataFrame and .xlsx

Best practive is to use a tool like *Zotero* (https://www.zotero.org/) to store all your papers etc. and create a .bib file of them. Using the *betterbibtex* extension (https://retorque.re/zotero-better-bibtex/installation/) allows to create an auto-updating .bib file from Zotero.

After you have installed Zotero and the extensions following above links, right click on a folder in your library -> *export Collection* -> *Format: Better BibTex* -> check *Export Notes* and *Keep Updated* -> Select a file in this repo. If you want to keep default configs, name it "bibliography.bib". 

Now you have an auto-updating file with all metadata collected on all literature in your zotero folder.
In addition you can select entries in Zotero -> File -> *Export PDF* and save them to pdf folder in this repo.

You can now open the parser.ipynb notebook and execute it. The .bib file will be transformed in a DataFrame with the columns you specify.
In addition, the DataFrame is exported to a nicely formatted .xlsx file:

![image](https://user-images.githubusercontent.com/65038289/224547900-406ae2b8-9f23-4a28-84e9-9da939e1ab16.png)

There is also a column *note* in the file, in which you can add custom info about the paper. This column will not be overwritten when you add entries to the .bib file and re-parse it.

This repo is already populated with papers on transformer models and especially VDU (Visual Document Understanding) to have a complete example of the module usage.
