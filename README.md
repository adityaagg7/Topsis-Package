# Topsis-Package

## A simple package to implement TOPSIS .

<br/>


## Installation:

        pip install Topsis-Aditya-102003706

</br>
 
# Command Line Usage


## USAGE:

        TOPSIS <input_data_file> <weight> <impact> <output_file>

_input_data_file_ :  The path of the CSV file that contains the input data. Sample input file is available on [github.](https://github.com/adityaagg7/Topsis-Package)</br></br>

_weight_ : The comma separated weights to be assigned to all the choices. Have to be same size as the data.  
eg:

        "1,1,1,1,1"
</br>
_impact_ :  The comma separated impacts to be assigned to all the choices. Have to be same size as the data.   
eg:  

        "+,-,+,-,+"
</br>

_otuput_file_ :  The path of the CSV file that will contain the result. Sample file is available on [github.](https://github.com/adityaagg7/Topsis-Package)

Example:

        TOPSIS Sample.csv "1,1,1,1,2" "+,-,+,-,+" Result.csv
</br>

# Usage as a Library

## Import:

        from Topsis.TOPSIS import topsis

## Syntax:

        topsis( input_data_file ,weight, impact, output_file )
</br>

## Returns:
A pandas dataframe containg the original data with the columns for Topsis Score appendt and Rank appended.
