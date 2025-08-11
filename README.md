# eTRM Data Download
This will proivded utilties to download measure package data (i.e., permutations) so you can use it for analysis in your Jupyter notebook

## Step 1: Obtain/set your unique eTRM token
Refer to "Authentication Headers" in the eTRM API user guide:
https://www.caetrm.com/media/user-guide-documents/eTRM_API_Specification_20230110_Px55ByC.pdf

For added security, store your token using MS Windowns command prompt : `setx CAE_TRM_TOKEN   "yourtoken"`

or, you can hard code "yourtoken" directly into the script

## Step 2: Install Packages

` %pip install requests ` 

` %pip install pandas `

` %pip install json `

## Step 3: Input the Measure Codes you Want

Input the measure code and version number after `codes =` like in example below:

` codes = [
    "SWWH027/06","SWWH025/09",
    # add the rest of your codes here …
] `

## Step 4: Analysis

The dataframe of permutations will be here: `measures_df`

