# Update Overview

#### 2021-01-30

- Added option to ignore files with `--ignore`

#### 2020-12-04
- Adjusted for new naming convention: `firstname-lastname` instead of `lastname-firstname`

#### 2020-11-22
- Now autodetects main notebook, as well as optionally commented and cross-commented notebooks.
- Removed the `notebook` parameter.

# How to use create_handin.py

First, edit the file and exchange our Team names with your Team names (first couple lines of `main()`).

Ensure your current working directory is one level **up** from the exercise directory.
Then, simply run the script with `python create_handin.py <exercise name>`.

The exercise directory must be named the same as what you want the hand-in to have at
the end. There must be one `*.ipynb` file in the directory, and optionally one `*-commented.ipynb`
as well as optionally one `*-cross-commented.ipynb` file.
You can compare your file structure to the one of this repository.

You can add more files to the hand-in by specifying a glob pattern in the `--more` option.

If your exercise directory contains extra notebooks, or you want to exclude certain files
from the `--more` option, you can do so with the `--ignore` option.

You can view more information about the tool using `python create_handin.py -h`.

The script assumes you have both a python 3 interpreter as well as jupyter added to your environment variables.
It was tested on Windows 10, using Python 3.8.

#### Example:
Current working directory: `SomeDir/FML/`

`python create_handin.py ex01a`


### Disclaimer: I do not take responsibility for your hand-in points if you use this tool, even if you use it correctly. Always double check your hand-in zip files.