# FIN: Function Inlining Neutralizer

[![GitHub license](https://img.shields.io/badge/license-Apache%202-blue.svg)](LICENSE)

## Project Description

This repository hosts the tool developed for the FIN paper, designed to construct a ground truth inlining dataset. The tool analyzes and compares the debug information of two ELF binaries to identify function calls from the first binary that have been inlined into the second binary.

## Installation

To set up the project, run the following command:

```bash
python setup.py
```

## Usage
To detect function inlining, you need two ELF files of the same program, but compiled with different optimization levels or compilers for comparison. Then, you can then run the following command, where `-o` specifies the path to the original binary file (from which function calls are extracted), and `-t` specifies the target binary file (in which inlined function calls are identified).
```bash
python fin.py -o /path/to/the/original/binary -t /path/to/the/target/binary
```

## Disclaimer

The software is provided as-is with no warranty or support. We do not take any responsibility for any damage, loss of income, or any problems you might experience from using our software. If you have questions, you are encouraged to consult the paper and the source code. If you find our software useful, please cite our paper above.

## Citation

If you use this code, please cite the following paper:

```bibtex
@article{yourlastname2024,
  title={Your Paper Title},
  author={YourLastName, FirstName and CoAuthorLastName, CoAuthorFirstName},
  journal={Journal Name},
  year={2024},
  volume={XX},
  number={YY},
  pages={ZZZ-AAA},
  doi={Your DOI},
  url={https://yourpaperlink}
}


