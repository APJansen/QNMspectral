# QNMspectral

A Mathematica package for the numerical computation of quasinormal modes.

## Citation

If one uses this code in any way in the preparation of a publication, please cite it as:

@article{Jansen:2017oag,
      author         = "Jansen, Aron",
      title          = "{Overdamped modes in Schwarzschild-de Sitter and a
                        Mathematica package for the numerical computation of
                        quasinormal modes}",
      journal        = "Eur. Phys. J. Plus",
      volume         = "132",
      year           = "2017",
      number         = "12",
      pages          = "546",
      doi            = "10.1140/epjp/i2017-11825-9",
      eprint         = "1709.09178",
      archivePrefix  = "arXiv",
      primaryClass   = "gr-qc",
      SLACcitation   = "%%CITATION = ARXIV:1709.09178;%%"
}

## Getting Started

These few steps will allow you to use this package.

### Prerequisities

Mathematica 10 or later is required for this package to work.

### Installing

1. If you haven’t already dowloaded it, click ‘Clone or download’ on the top right, and choose `download ZIP`.

2. Now copy the ‘QNMspectral’ folder (not 'code', this is used only to create the documentation).

3. Paste this folder into the folder 'Applications' located in the Mathematica user base directory. 
   To find the location of this user base directory, open a Mathematica notebook and evaluate ‘$UserBaseDirectory’.
   On a Mac this will be in the 'library' folder, which is hidden by default, to acces that in Finder click Go->Go to Folder... and type '/Library'.
   
4. To get the documentation to work, reset Mathematica.

### Loading

The package is now installed. To use it in a notebook of your own, you first have to load it, by evaluating:

Needs\["QNMspectral\`"\] 

### Using

Once it is loaded, one can go to Help->Wolfram Documentation and type in ‘QNMspectral’ to get a usage guide.

Alternatively, there is a notebook with examples in the main folder, titled ‘QNMspectralExamples.nb’.

## Contributing

If you wish to contribute to the package, for example by fixing a bug or even adding a feature, you are welcome to do so.

The source code is located in the code/QNMspectral folder. 
This can be used with Wolfram Workbench to create the package with documentation included.
The actual code is QNMspectral.m, which is created from QNMspectral.nb.

## Authors

Aron Jansen

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

### Changes with respect to pre-github version

#### Summary of changes with respect to the pre-github version

1. Added Mathematica-style documentation, with an information page for each function, and some tutorials.
2. Some significant speed improvements (most notable with machine precision and small grids, with around a factor 6 speedup)
3. Fixed several bugs
4. To more closely match Mathematica’s conventions, removed quotation marks from all option names, and added $ sign to global option variables ($QNMMemory and $QNMQuiet)
5. Restructured most of the code, to make it more readable and more modular

##### Backwards compatibility

For anyone who has used the pre-github version, there are two changes you have to make to any old code to make it compatible with the current version:

1. Remove all quotation marks from option names (not from their values)
2. Add a $-sign to any use of QNMMemory and QNMQuiet.


[![Analytics](https://ga-beacon.appspot.com/UA-81215073-4/chromeskel_a/readme)](https://github.com/QNMspectral/ga-beacon)
