# Build
### Install OpenCascade Community Edition
```
cd Deps/oce
mkdir build
cd build
cmake ..
make -j8
make test # Not required.
make install
```

### Install FreeCAD
```
apt-get install freecad
```

### Install ToPy
```
conda create -n CADO
conda install -f conda.yaml
conda activate CADO
cd Deps/topy
python setup.py install
```

### Build CADO
```
conda activate CADO
cd CADO
make
```
