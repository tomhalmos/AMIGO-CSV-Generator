# AMIGO-CSV-Generator

The code will generate the CSV file for DNA-BOT taking three ORFs and desired gene ratios as inputs. Unless specified, the plasmid, promoter and UTRs will have default settings.

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
