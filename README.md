# hawk

A simple command line histogram tool written in AWK.


# Examples

```
$ python -c "from __future__ import print_function; import numpy; [print(int(round(i))) for i in numpy.random.normal(loc=100.0, scale=10.0, size=1000)]" | sort -n | ./hawk
IQR  14
Bin Size  2
MIN||MAX::  63 || 135
Total bins:  43.5
Length of xs  1000  and total lines  1000
Displaying histogram: 

  RANGE   ||  COUNT

=================================================================================================================

< 2       || 
< 4       || 
< 6       || 
< 8       || 
< 10      || 
< 12      || 
< 14      || 
< 16      || 
< 18      || 
< 20      || 
< 22      || 
< 24      || 
< 26      || 
< 28      || 
< 30      || 
< 32      || 
< 34      || 
< 36      || 
< 38      || 
< 40      || 
< 42      || 
< 44      || 
< 46      || 
< 48      || 
< 50      || 
< 52      || 
< 54      || 
< 56      || 
< 58      || 
< 60      || 
< 62      || 
< 64      || **
< 66      || 
< 68      || 
< 70      || 
< 72      || ***
< 74      || **
< 76      || ***********
< 78      || *********
< 80      || *****************
< 82      || ***********************
< 84      || *****************
< 86      || ****************************
< 88      || ********************************************
< 90      || **********************************************
< 92      || ***********************************************************
< 94      || ***************************************************************************
< 96      || ***********************************************************************************
< 98      || ****************************************************************************
< 100     || ***********************************************************************************
< 102     || ****************************************************************************************
< 104     || ****************************************************************************************************
< 106     || **************************************************************************************************
< 108     || ******************************************************************************
< 110     || ****************************************************************
< 112     || **************************************************
< 114     || ****************************************
< 116     || ***********************
< 118     || ***************
< 120     || *************
< 122     || *******
< 124     || **
< 126     || **
< 128     || **
< 130     || **
< 132     || ***
< 134     || 
< 136     || **
```

# TODO

  * bucket around data rather than starting from zero
  * add CLI options for width and what not
  * add axis ticks for histogram width
  * add horizontal histogram
  * cleanup awkward 0/1 indexes
  * support negative values
  * sort data?
  * Support non even quantities of data
