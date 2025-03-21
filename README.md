# CIF to PDB Converter

## Overview
This script converts Crystallographic Information Files (`.cif`) to Protein Data Bank format (`.pdb`) recursively within a specified directory. Converted `.pdb` files are saved both in their original locations and in an organized output folder.

## Requirements
- Python 3.x
- Biopython

Install Biopython via pip:
```bash
pip install biopython
```

## Usage

### Running the Script

Execute the Python script from your command line:

```bash
python cif_to_pdb_converter.py
```

You will be prompted to input the path to the directory containing `.cif` files:

```bash
Enter the path to the input folder: "C:/path/to/cif_files"
```

### File Organization

Upon completion, `.pdb` files will be available:
- In the original `.cif` file locations.
- In a structured `output` subdirectory created within your specified input folder, preserving the folder hierarchy.

```
input_folder/
├── example1.cif
├── example1.pdb
├── subfolder
│   ├── example2.cif
│   └── example2.pdb
└── output
    ├── example1.pdb
    └── subfolder
        └── example2.pdb
```

## Error Handling
The script gracefully handles conversion errors, notifying users of any files that fail to convert, along with the corresponding error message.

## License
This project is available under the MIT License.

---
**Author:** Ryeogang Son
**Contact:** pulzang@gmail.com (rg.son@nus.edu.sg)
