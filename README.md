# AMIGO-CSV-Generator

The code will generate the CSV file for DNA-BOT taking three ORFs and desired gene ratios as inputs. Unless specified, the plasmid, promoter and UTRs will have default settings.

So I've made one Python file and will add it to this repository. Pick a task from the below, fork the Python file, work on your code and then when it's ready, merge it into the master file. If your bit of code needs inputs from another bit just input your own variables when testing it and we'll sort that out when we stitch it all together. If anyone (Will) knows a better way to use GitHub pls explain aha. 

Code needs to be written to:
1) Take three ORFs and the gene ratios as user input
  -- Allow input of PDB ID?
  -- Take desired gene ratio and return the correct combination of RBSs (from the sfGFP RBS ranking data)
2) Allow user to change plasmid, promoter and UTR defaults if they want (select from BASIC part list)
3) Take the ORFs, RBSs, plasmid, promoter and UTRs and return the official CSV names from the BASIC part list
  -- The ORFs won't be in the part list (Use a temporary name, until part can be added to registry in the future)
4) Create a CSV file with 1 line (no combinations)
  -- Add the LMP/LMS linkers, make sure the ORFs are added with the correct RBS
5) Take the one line CSV and generate all possible combinations
  -- Keeping RBS with ORF
  -- Plasmid/promoter parts don't move


