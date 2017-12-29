[![Build Status](https://travis-ci.org/PyORBIT-Collaboration/laser-stripping.svg?branch=master)](https://travis-ci.org/PyORBIT-Collaboration/laser-stripping)
# Laser stripping extension for pyORBIT code
Installation procedure requires building from source.
All installation steps happen in command line (terminal). 

 ## 1. Build pyORBIT as described [here](https://github.com/PyORBIT-Collaboration/py-orbit)
 ## 2. Clone the source code
```shell
git clone https://github.com/PyORBIT-Collaboration/laser-stripping.git
```
Put the cloned repository somewhere outside of pyORBIT directory.
So your source is now in *laser-stripping* directory.

## 3. Setup environment variables
If you built pyORBIT environment from source, use *customEnvironment.sh* instead.
```shell
source <path-to-pyORBIT-installation>/setupEnvironment.sh
```
## 4. Build the code

```shell 
make clean
make
```
This will put a dynamic library into *\<path-to-pyORBIT-installation\>/lib*.
If make failed, it usually means that some of the libraries aren't set up properly.

# Running Examples
 
```shell
cd examples
./START.sh 1GeV-particle-stripping.py 2
```
This will launch *1GeV-particle-stripping.py* example on two MPI nodes. Other laser stripping related examples are availabale in [Examples](https://github.com/PyORBIT-Collaboration/examples/tree/master/ext/LaserStripping) repository.
