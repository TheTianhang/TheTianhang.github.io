---
layout: archive
title: "How to run MD simulations"
permalink: /mds/
author_profile: true
redirect_from:
  - /resume
---

How to run MD simulation?

I. Preparation all softwares(Linux):

  **Moltemplate**

    Install Moltemplate: [https://www.moltemplate.org/download.html]

Comments: easy process in linux. git clone https://github.com/jewettaij/moltemplate moltemplate

  **Packmol**

    Install packmol: [http://leandro.iqm.unicamp.br/m3g/packmol/download.shtml]

Comments: Fill your email and then download

  **Lammps**

    Install Lammps: [https://lammps.sandia.gov/download.html]

Comments: The simplest way is to use cmake.


    cd lammps                # change to the LAMMPS distribution directory
    mkdir build; cd build    # create and use a build directory
    cmake ../cmake           # configuration reading CMake scripts from ../cmake
    cmake --build .          # compilation (or type "make")


II. Simulation

Following the first example https://www.moltemplate.org/examples.html 

  Download all files then:

    moltemplate.sh system.lt

    lmp_mpi -i run.in.npt