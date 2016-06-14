ScatterAlloc
============

ScatterAlloc: Massively Parallel Dynamic Memory Allocation for the GPU

This project provides a **fast memory manager** for **Nvidia GPUs** with
compute capability `sm_20` or higher.

From http://www.icg.tugraz.at/project/mvp/downloads :
```quote
ScatterAlloc is a dynamic memory allocator for the GPU. It is
designed concerning the requirements of massively parallel
execution.

ScatterAlloc greatly reduces collisions and congestion by
scattering memory requests based on hashing. It can deal with
thousands of GPU-threads concurrently allocating memory and its
execution time is almost independent of the thread count.

ScatterAlloc is open source and easy to use in your CUDA projects.
```

Original Homepage: http://www.icg.tugraz.at/project/mvp

Our Homepage: https://www.hzdr.de/crp


Further Development
-------------------

Please visit our
[fork](https://en.wikipedia.org/wiki/Fork_%28software_development%29)
of this project: [mallocMC](https://github.com/ComputationalRadiationPhysics/mallocMC)

**mallocMC** includes a major redesign of the library.
Starting from a policy based design for general memory pools, we implemented a whole new environment and plenty of features.
Of course, the *scatterAlloc* algorithm is implemented, too.


About This Repository
---------------------

This repository is a clone of the **ScatterAlloc** project from the
[Managed Volume Processing](http://www.icg.tugraz.at/project/mvp)
group at [Institute for Computer Graphics and Vision](http://www.icg.tugraz.at),
TU Graz (kudos!).

We fixed and backported ~~minor~~ bugs we found while developing
[mallocMC](https://github.com/ComputationalRadiationPhysics/mallocMC)
to this repository.


Literature
----------

Just a random link collection:

- [Paper](http://www.icg.tugraz.at/Members/steinber/scatteralloc-1) by
  Markus Steinberger, Michael Kenzel, Bernhard Kainz and Dieter Schmalstieg

- 2012, May 5th: [Presentation](http://innovativeparallel.org/Presentations/inPar_kainz.pdf)
        at *Innovative Parallel Computing 2012* by *Bernhard Kainz*


License
-------

We distribute the modified software under the same license as the
original software from TU Graz (by using the
[MIT License](https://en.wikipedia.org/wiki/MIT_License)).
Please refer to the [LICENSE](LICENSE) file.
