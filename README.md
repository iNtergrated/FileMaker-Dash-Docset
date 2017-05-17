FileMaker Pro 16
=======================

* [Jason P. Scharf](https://github.com/iNtergrated/) [@jpscharf](https://twitter.com/jpscharf)

## Docset Generation ##

1. Clone the docset generation [repository](git@github.com:iNtergrated/FileMaker-Dash-Docset.git): ````git clone git@github.com:iNtergrated/FileMaker-Dash-Docset.git````

2. For FileMaker < 15, use master, otherwise checkout the branch for your version, e.g. `checkout FileMaker-16`
3. Download the FileMaker Help File: `http://www.filemaker.com/redirects/fmp16_admin.html?page=help_zip&lang=en`
4. Extract the zip file, rename the folder to `FileMaker Help`, and copy to the root of this folder.
5. Install dependencies: ````composer install````
6. Generate the docset: ````php generate````
7. The generated docset can be found inside the build folder: ````build/FileMaker.docset````
