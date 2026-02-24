
I am putting it here a package and deployment I have done while working in the University of Sheffield. I am charged with reorganised the code and make it into a package, which is published here https://pypi.org/project/retrodetect/. Concept belongs to the researcher, and in view of the potential changes in the future, I am just duplicating the code here, rather than forking it. https://pypi.org/project/retrodetect/


# Bee retroreflection detector

Detect retroreflectors in image pair.

# Installation

```bash
pip install retrodetect
```

# Usage
The `detectcontact` function in this package analyzes a sequence of photos captured by a tracking system to detect potential retroreflectors with the `detect` function capturing the differences (retro-reflectors) detected between the flash and no flash images.
See examples for details.

```python
from retrodetect import detect, detectcontact

contact,found,searchimg = detectcontact(photo_list,n,delsize=100)

output = detect(flash,noflash,blocksize=20, offset=10, searchbox=20, step=4, searchblocksize=50, ensemblesizesqrt=3, dilate=True,margin=100)
```

## Contributing

Interested in contributing? Check out the [contributing guidelines](https://github.com/SheffieldMLtracking/.github/blob/main/CONTRIBUTING.md). 
Please note that this project is released with a Code of Conduct. 
By contributing to this project, you agree to abide by its terms.
