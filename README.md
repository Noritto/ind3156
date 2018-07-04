# ind3156
for class

Take the dataset from World Value Survey from Wave 6 on Russia and open it in python.

Stata files available on Russia had extensions: .dat, .dct and .do
The spss available - .sav

Tried with .dat, using numpy, however, had a problem with the value enter in one colume "1-4', which oython could not process. 
The other problem with numpy was recording whitespace as a separator, but some of them numpy did not take into account, therefore, some data points were shifted, and it couldn't read different quantities of values in different rows.

Pandas also read a similar error

Found out that it is easier to do with .dta file. Opened it. Looked good

.dta file available on World Value survey website was for all countries in that wave, but my aim was to get Russia, therefore, with pandas sliced the file, using criteria to put in the new datafram only rows that have the code of Russia in column 2.

Saved this file using df.to_stata command on the computer.

Oepned in the new notebook, it worked, got the file that was needed for em
