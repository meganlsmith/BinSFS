# BinSFS
Create a binned version of the SFS

Introduction:
SFS_CreateBinned.py will coarsen a multidimensional SFS to include a user-defined number
of classes per population. This script is written in python 2.7 and works for four populations.

Input: 
As input, SFS_CreateBinned.py requires two things: 
1.  The user must provide a SFS. If this SFS was constructed using Jordan Satler's 
    downsampling script (https://github.com/jordansatler), the user must specify the 
    threshold used. 
2.  The user must provide a TRAITS file. This file should be a tab-delimited file. The
    first line should be the headers traits\t species. In the first column, list the names
    of the individuals sampled (as they are listed in your SFS). In the second column, 
    list the population each individual belongs to.

Usage: 
The required arguments are as follows, in the specified order
script,Traits,file,Threshold,classes,outfile = argv #arguments the user must supply

example usage:
python SFS_CreateBinned.py TRAITS.txt Example_SFS.txt 50 4 Binned_SFS.txt

Output: 
The script will create a SFS with the desired number of questions.

If you have any questions or comments, please email me at megansmth67@gmail.com.

Please refer to: Smith ML, Ruffley MR, Espíndola AE, Tank DC, Sullivan J, Carstens BC. Demographic model selection using random forests and the site frequency spectrum. Molecular Ecology.
