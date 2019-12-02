# AMIGO-CSV-Generator

The code will generate the CSV file for DNA-BOT taking five ORFs and desired gene ratios as inputs. Unless specified, the plasmid, promoter and UTRs will have default settings.

So I've made one Python file and will add it to this repository. Pick a task from the below, fork the Python file, work on your code and then when it's ready, merge it into the master file. If your bit of code needs inputs from another bit just input your own variables when testing it and we'll sort that out when we stitch it all together. If anyone (Will) knows a better way to use GitHub pls explain aha. 

INPUT: PDB IDs (Up to 5) + Desired Ratio
OUTPUT: BASIC sequences for synthesis + CSV file for DNA BOT

Code needs to be written to:
TOM: 1) Take up to five ORFs as PBD IDs as user input and reuturn BASIC sequence
      -- Look up sequence in PBD
      -- Add standardised prefix/suffix sequences
      -- ADDITION: we need to search the sequence for any internal BsaI sites and remove them!
      -- Generate standardised name
      -- Add to a local registry of parts
     2) Take the desired gene ratio as input 
      -- Figure out best way to input this (same order as PBD IDs?)
      -- Using sfGFP data find combination of RBSs
      -- Return standardised name for RBSs + UTR(1-5)
    3) Allow user to change plasmid, promoter if they want
    -- Promoter can be selected from weak, medium or strong
    -- Plasmid can be selected based on antibiotic resistance and/or copy number
    4) Create a CSV file with 1 line (no combinations)
      -- Add the LMP/LMS linkers, make sure the ORFs are added with the correct RBS
    5) Take the one line CSV and generate all possible combinations
      -- Keeping RBS/UTR with ORF
      -- Plasmid/promoter parts don't move
      -- Return CSV file and BASIC sequences (email to user?)


