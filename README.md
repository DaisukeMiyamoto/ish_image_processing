ish\_image\_processing
=====

Tools for formatting Marmoset in situ hybridization images


## Requirement
<!--
 - ImageJ
 - Download "Bio-Formats Package" and "Command Line Tools" from [here](http://downloads.openmicroscopy.org/bio-formats/5.1.10/) and put them to ``ImageJ/plugins/``
-->
- Install Fiji
- Add this line to your .bashrc (not necessary but used in the following description): 
```
alias imagej='/Applications/Fiji.app/Contents/MacOS/ImageJ-macosx'
```

## Usage
### ConvertSCNtoTIFF.txt
Makes  ``filename.scn_rough.tiff`` from ``filename.scn``
### 
```
$ imagej -macro ish_image_processing/ConvertSCNtoTIFF.txt [target_directory]
```

### Trimming.txt
Trim three images for each slide

Makes  ``filename.scn_rough-[i].tiff`` from ``filename.scn_rough.tiff`` where [i] = 1,2,3
```
$ imagej -macro ish_image_processing/Trimming.txt [target_directory]
```