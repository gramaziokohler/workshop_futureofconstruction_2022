# Future of Construction Symposium: Computational Design with COMPAS

> Crash course to **understand** the available components to **computational design and robotic fabrication** using COMPAS

## Information

[COMPAS docs](https://compas.dev)

## Requirements

* Minimum OS: Windows 10 Pro or Mac OS Sierra 10.12
* [Anaconda 3](https://www.anaconda.com/distribution/)
* [Rhino 6/7 & Grasshopper](https://www.rhino3d.com/download)

Optional:

* [Docker Desktop](https://www.docker.com/products/docker-desktop) After installation on Windows, it is required to enable "Virtualization" on the BIOS of the computer.
* [Visual Studio Code](https://code.visualstudio.com/): Any python editor works, but we recommend VS Code + extensions [as mentioned in our docs](https://gramaziokohler.github.io/compas_fab/latest/getting_started.html#working-in-visual-studio-code-1)

## Installation

We use `conda` to make sure we have clean, isolated environment for dependencies.

<details><summary>First time using <code>conda</code>?</summary>
<p>

Make sure you run this at least once:

    (base) conda config --add channels conda-forge

</p>
</details>

    (base) conda env create -f https://dfab.link/fc22.yml

### Add to Rhino

    (base) conda activate fc22
    (fc22) python -m compas_rhino.install -v 7.0

### Get the workshop files

    (fc22) cd Documents
    (fc22) git clone https://github.com/gramaziokohler/workshop_futureofconstruction_2022.git

### Verify installation

    (fc22) python -m compas

    Yay! COMPAS is installed correctly!

    COMPAS: 1.16.0
    Python: 3.9.10 | packaged by conda-forge | (default, May 11 2021, 06:25:23) [MSC v.1916 64 bit (AMD64)]
    Extensions: ['compas-fab', 'compas-cgal', 'compas-rrc']

### Update installation

To update your environment:

    (fc22) conda env update -f https://dfab.link/fs2022.yml
