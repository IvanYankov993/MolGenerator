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


# PA - DNA 3D Complex Generator for NMR-informed rMD Refinement

## Overview
PA-DNA 3D Complex Generator is a Python-based library designed for generating DNA-protein complex structures informed by Nuclear Magnetic Resonance (NMR) data and refined using restrained Molecular Dynamics (rMD) simulations. This toolkit provides functions to build, manipulate, and refine DNA and peptide complexes, enabling the creation of accurate 3D models based on experimental data. It supports a variety of features including the generation of 3D structures, conformational searches, and complex formation via docking protocols.

## Key Features

### PA (Peptide/Protein Assembly)
- **User-Defined Fragment Repository/Dictionary:** Build peptide/protein structures based on user-specified fragment libraries.
- **Linear Builder:** Utilize user-defined rules of SMILES strings for combinatorial search and dataset creation. The builder allows for input interpretation and flexible peptide design.
- **RDKIT Functionality:** Automatically generate 2D structural representations (drawings) of peptides/proteins using SMILES strings.
- **SMILES to 3D Generator:** Convert SMILES notation into 3D structures for peptides and other small molecules.

### DNA (Deoxyribonucleic Acid)
- **Web-Based 3D DNA Generation:** Leverage online tools to generate 3D structures from DNA sequences.
- **Combinatorial DNA Sequence Generation:** Create unique DNA sequences based on a template with customizable iterative positions (e.g., AGCTWWWTCGA).
  - **Identify Unique DNA Sequences**
  - **Identify Palindromic Sequences**
  - **Consider Directionality:** Account for 5'-3' vs 3'-5' orientations.
- **Dataset Curation:** Collect and organize unique DNA sequences for further analysis.
- **Molecular Dynamics (MD) Screening:** Perform unrestrained MD simulations on DNA 3D structures.
- **Experimental Comparison:** Compare simulated DNA structures with experimentally obtained data (X-ray and NMR).

### Conformational Search
- **DNA Search Space Identification:** Expand the minor groove based on experimentally derived data.
- **PA Search Space Identification:** Define the search space for peptide/protein conformations using specific volume and dihedral angle combinations.
- **Conformation Search Methods:** 
  - Use MD simulations based on P-P distances for DNA templates and peptide dihedral angles.
  - Apply geometry optimization techniques such as RMSD analysis and others for better conformation refinement.

### Complex Formation and Docking Protocol
- **Docking Protocols:**
  - **Hard Docking:** Target drug molecules to the protein/DNA complex.
  - **Hard-Soft Docking:** Hybrid docking approach combining hard and soft interactions for more accurate docking.
  - **Soft-Soft Docking:** Fully flexible docking of target drug molecules to the protein/DNA complex.

### Integration with NMR-MD-MARDI Workflow and SPARKY Visualization Tool
The toolkit is designed to work seamlessly with the NMR-MD-MARDI workflow and can be visualized using the SPARKY model visualization tool.

### Output
- **PDB File Generation:** The library generates output in the PDB format, with consistent labels and properly formatted 3D models.

## Installation
To install the PA-DNA 3D Complex Generator, simply clone the repository and install the dependencies:

