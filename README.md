# MolGenerator
PA - DNA 3D Complex Generator for NMR informed rMD refinement


Elements in this library include:

PA
[1] User defined Fragment repository/dictinary for building PA
[2] Linear builder (user defined rules of SMILES strings, allowing for user input interpretation and combinatorial search " dataset creation"
[3] RDKIT function for generating 2D drawings
[4] SMILES to 3D generator

DNA
[1] Python function for utilising web 3D DNA generators from sequence
[2] Python function for generating unique DNA combinatorial seqeunce based on a tempalte with iterating position W e.g. AGCTWWWTCGA
  [2.1] Identify unique DNA sequences
  [2.2] Identify palindromic sequences
  [2.2] Consider directionality 5'-3' vs 3'-5'
[3] Data set curation
[4] MD screening of 3DNA unrestrained simulation
[5] Comparison of [4] with experimental DNA structures X ray and DNA compelx free.

Conformational search
[1] Identify search space for DNA (always expanded minor groove) experimentaly derived 
[2] Identify search space for PA (specific volume, a set of Dihedral angles and their combinaitons) experimentaly derived
[3] Conformation searhc method - MD using P-P distances on DNA tempaltes, and others ? as well as PA on the dihedrals
[4] Conformation search methods - Geometry optimisaition ?, RMSD and others

Complex formation Docking protocol
[1] Hard docking      Target - drug
[2] Hard-soft docking Target - drug
[3] soft-soft docking Target - drug

#This ties into NMR-MD-MARDI workflow and SPARKY MODEL VISUALISATION TOOL

Output must be a PDB file (with consistent labels)
