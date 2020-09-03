Bootstrap: docker
From: debian:stretch-slim

%labels
Author "Randall Cab White - rcwhite@stanford.edu"


#########
#%setup
#########

#Downlaod packages
%post
  apt-get -ym update
  apt-get -ym install build-essential curl wget git
  
### Spack stuff 
git clone https://github.com/spack/spack.git

#cd into spack directory:
cd spack*

#deps


#toolchain
./bin/spack install gcc
./bin/spack install gdb
./bin/spack install rr
./bin/spack install autoconf
./bin/spack install autogen
./bin/spack install automake
./bin/spack install gmake
./bin/spack install cmake
./bin/spack install openmpi
./bin/spack install openjdk
./bin/spack install jemalloc
./bin/spack install lbzip2
./bin/spack install zip
./bin/spack install adios
./bin/spack install adios2
./bin/spack install parallel
./bin/spack install tcl
./bin/spack install tk
./bin/spack install perl
./bin/spack install sz
./bin/spack install trilinos
./bin/spack install vtk
./bin/spack install wrf
./bin/spack install xios
./bin/spack install yambo
./bin/spack install harfbuzz
./bin/spack install qt
./bin/spack install rclone
./bin/spack install readline
./bin/spack install rsync
./bin/spack install neovim
./bin/spack install sox
./bin/spack install emacs
./bin/spack install exa
./bin/spack install intel
./bin/spack install intel-parallel-studio

#math libraries
./bin/spack install lapackpp
./bin/spack install libflame
./bin/spack install fftw
./bin/spack install cblas
./bin/spack install openblas
./bin/spack install atlas

#text libraries
./bin/spack install json-c
./bin/spack install jsoncpp
./bin/spack install pandoc

#graphics
./bin/spack install opengl
./bin/spack install openglu
./bin/spack install freeglut
./bin/spack install openjpeg
./bin/spack install libjpeg-turbo
./bin/spack install pango
./bin/spack install ffmpeg

#earth sciences
./bin/spack install netcdf-c
./bin/spack install netcdf-fortran
./bin/spack install  netcdf-cxx
./bin/spack install  netcdf-cxx4
./bin/spack install  parallel-netcdf
./bin/spack install  nccmp
./bin/spack install  ncl
./bin/spack install  nco
./bin/spack install  cgal
./bin/spack install  ncview
./bin/spack install gdal
./bin/spack install geos
./bin/spack install gdl
./bin/spack install gmt
./bin/spack install grads
./bin/spack install grass
./bin/spack install grib-api
./bin/spack install hc
./bin/spack install ibmisc
./bin/spack install magics
./bin/spack install mfem
./bin/spack install moab
./bin/spack install octopus
./bin/spack install lammps
./bin/spack install paraview
./bin/spack install petsc
./bin/spack install pism
./bin/spack install abinit
./bin/spack install accfft
./bin/spack install asagi
./bin/spack install cdo
./bin/spack install channelflow
./bin/spack install cmor
./bin/spack install esmf
./bin/spack install ferret
./bin/spack install fortrilinos
./bin/spack install fpocket
./bin/spack install fstrack
./bin/spack install qgis
./bin/spack install regcm
./bin/spack install seacas
./bin/spack install siesta
./bin/spack install proj

# python stuff
./bin/spack install python
./bin/spack install py-pip
./bin/spack install py-markdown
./bin/spack install py-abipy
./bin/spack install py-arviz
./bin/spack install py-cdat-lite
./bin/spack install py-cdo
./bin/spack install py-cftime
./bin/spack install py-dxchange
./bin/spack install py-mdanalysis
./bin/spack install py-netcdf4
./bin/spack install py-pynio
./bin/spack install py-pyugrid
./bin/spack install py-wradlib
./bin/spack install py-gdal
./bin/spack install py-slurm-pipeline
./bin/spack install  py-basemap
./bin/spack install  py-pillow
./bin/spack install  py-scipy
./bin/spack install  py-pyproj
./bin/spack install  py-matplotlib
./bin/spack install py-seaborn
./bin/spack install py-selenium
./bin/spack install py-plotly
./bin/spack install py-pandas
./bin/spack install  py-rpy2
./bin/spack install   py-torch
./bin/spack install  py-torch-geometric
./bin/spack install   py-xarray
./bin/spack install  py-cartopy
./bin/spack install  py-mpi4py
./bin/spack install  py-protobuf
./bin/spack install  py-tblib

#r stuff
./bin/spack install r
./bin/spack install r-mzr
./bin/spack install r-geomorph
./bin/spack install r-viridis
./bin/spack install r-geonames
./bin/spack install r-geoquery
./bin/spack install r-geor
./bin/spack install r-geosphere
./bin/spack install r-gdalutils
./bin/spack install r-ggmap
./bin/spack install r-ggplot2
./bin/spack install r-plotly
./bin/spack install r-proj
./bin/spack install r-proj4


#julia
./bin/spack install julia


#tensorflow
./bin/spack install py-tensorflow
./bin/spack install py-tensorflow-estimator
./bin/spack install py-tensorboard
./bin/spack install py-tensorboard-plugin-wit
./bin/spack install py-tensorboardx

#jupyterlab
./bin/spack install py-jupyterlab
./bin/spack install py-jupyterlab-server

#keras
./bin/spack install py-keras
./bin/spack install py-keras-applications
./bin/spack install py-keras-preprocessing

#nlp
./bin/spack install py-spacy

#pip
pip3 install ipyvolume metpy lagranto protobuf

##
##
##
##
##

%environment
#set up spack environment
export IMAGE_NAME="ipshita_mazama_image"
