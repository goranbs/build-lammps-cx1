# Building LAMMPS on CX1

Makefile.mpi is a mpi make file for LAMMPS on CX1.

build-lammps-cx1.pbs is a script that installs LAMMPS on the computing cluster.

What you need to do:

Upload the version of LAMMPS that you want from the sandia web page:
http://lammps.sandia.gov/download.html
to the computing cluster and place it somewhere convenient. For example:
$WORK/lammps-builds
Then upload build-lammps-cx1.pbs to the the top folder of your LAMMPS directory. E.g:

$WORK/lammps-builds/lammps-31Mar17/build-lammps-cx1.pbs

And put the make file into scr/MAKE/ then submit the pbs script:

qsub build-lammps-cx1.pbs
