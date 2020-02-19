# Build (Debian)
### Install OpenCascade Community Edition
```sh
cd Deps/oce
mkdir build
cd build
cmake ..
make -j8
make test # Not required.
make install
```

### Install FreeCAD
```sh
apt-get install freecad
```

### Install ToPy
```sh
conda create -n CADO
conda install -f conda.yaml
conda activate CADO
cd Deps/topy
python setup.py install
```

### Build CADO
```sh
conda activate CADO
cd CADO
make
```
