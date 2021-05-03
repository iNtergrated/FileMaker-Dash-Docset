FileMaker Pro 19
=======================

* [Jason P. Scharf](https://github.com/iNtergrated/) [@jpscharf](https://twitter.com/jpscharf)

## Docset Generation ##

1. Clone the docset generation [repository](git@github.com:iNtergrated/FileMaker-Dash-Docset.git): ````git clone git@github.com:iNtergrated/FileMaker-Dash-Docset.git````
https://www.filemaker.com/redirects/fmp19_admin.html?page=help_zip&lang=en
2. Download the FileMaker Help File: `https://help.claris.com/downloads/fmp-19-help-en.zip`
    > `curl -O https://help.claris.com/downloads/fmp-19-help-en.zip`
4. Extract the zip file, rename the folder to `FileMaker Help`, and copy to the root of this folder.
    > `unzip fmp-19-help-en.zip`
    > `mv en "FileMaker Help"`
5. Install dependencies: ````composer install````
6. Generate the docset: ````php generate````
7. The generated docset can be found inside the build folder: ````build/FileMaker.docset````


## Known Issues ##
- Native FileMaker help search does not work.