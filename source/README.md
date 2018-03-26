## Tajawal Open-Source Font

See: 

     /source/1-drawings/Tajawal-Black.ufo
     /source/1-drawings/Tajawal-Bold.ufo
     /source/1-drawings/Tajawal-Extrabold.ufo
     /source/1-drawings/Tajawal-Light.ufo
     /source/1-drawings/Tajawal-Medium.ufo
     /source/1-drawings/Tajawal-Regular.ufo
     /source/1-drawings/Tajawal-UltraLight.ufo

URW Beziér Format is used as source and production file format. The production is done with URW program IKED and OTM.
See: 

     /source/2-production/Tajawal-Black/Tajawal-Black.be
     /source/2-production/Tajawal-Bold/Tajawal-Bold.be
     /source/2-production/Tajawal-Extrabold/Tajawal-Extrabold.be
     /source/2-production/Tajawal-Light/Tajawal-Light.be
     /source/2-production/Tajawal-Medium/Tajawal-Medium.be
     /source/2-production/Tajawal-Regular/Tajawal-Regular.be
     /source/2-production/Tajawal-UltraLight/Tajawal-UltraLight.be


For each of the seven font weights the production of TTF and OTF is done with IKED and OTM using five additional ASCII-files as input:

* arab.cha (containing a glyph list of IKED used numbers and according UNICODES and PS names for the conversion from URW Beziér to OTF or TrueType)
* gdef.fea (containing the GDEF feature information)
* gpos.fea (containing GPOS feature information)
* gsub.fea (containing the GSUB feature information)
* Tajawal-Bold.ufm (URW font metric file, which contains all necessary name and other table entry information for the final font production)


Production:

In each font directory the five ASCII files (see above) and the Bezièr file must be present.

1. Start progeam IKED and select File/Open and open the Bezièr file
2. Select File/MakeOpenType Font
3. Select IMPORT the layout file "arab.cha"
4. Select "More" to change certain metric values
5. Select "Target font file"
6. Select "Make"


After production of the Basic Type format use program OTM to add the necessary feature files.











