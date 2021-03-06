# PLASM (Programming LAnguage for Solid Modeling)

Plasm is a 'design language' for geometric and solid parametric design, 
developed by the CAD Group at the Universities 'La Sapienza' and 'Roma Tre' in Italy. See also: http://www.plasm.net/

Supported python versions: >=3.6 (python 2.x no longer supported).

Supported OS: Windows, MacOsX, Linux. 

To install `pyplasm`

```
# For Linux sometimes you have to install some python libraries 
# sudo apt-get install python3.6 libpython3/6

# replace `python3` with your python executable path
python3 -m pip install --user --upgrade pip numpy GL PyGlut PyOpenGL 
python3 -m pip install --upgrade pyplasm
```

<!--
DISABLED: problems on github actions

If you are using `conda` python:

```
conda install numpy pyopengl freeglut
conda install -c conda-forge libglu # if this fails just ignore it
conda install --channel scrgiorgio pyplasm
```
-->

Then test it:

```
python3 -c "from pyplasm import *; VIEW(CUBOID([1,1,1]))"
```



<!--
////////////////////////////////////////////////////////////////////////
## Commit CI (only for developers

Edit file `src/xgepy/setup.py` and increment the VERSION.

```
TAG=...write the same value of VERSION here...
git commit -a -m "New tag" && git tag -a $TAG -m "$TAG" && git push origin $TAG && git push origin
```

 -->


