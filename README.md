## Tracking FreeCAD and Dependencies
This repository's function is to track FreeCAD and it's 3rd party dependencies in the package ecosystem

## Hot to bump versions or request new packages
<details>
  <summary><b>Expand this section in order to view it</b></summary>

### Arch Linux
1. Search for the package in: https://www.archlinux.org/packages/
2. On the package page find `Flag Package Out-of-Date` link

### Arch Linux User Repository (AUR)
1. Search for the package in: https://aur.archlinux.org
2. On the package page find `Flag Package Out-of-Date` link

### Chocolatey 
Request new packages at https://github.com/chocolatey/chocolatey-package-requests  
Request package updates by [contacting the maintainer of said chocolatey package](https://chocolatey.org/docs/package-triage-process#package-is-outdated)

### FreeBSD (aka Freshports/dports)
Open a ticket on their [Bugzilla](https://bugs.freebsd.org/bugzilla/enter_bug.cgi) bugtracker.  
FYI, dports lags behind Freshports 

### Gentoo
1. Open a ticket on their [Bugzilla](https://bugs.gentoo.org/enter_bug.cgi?product=Gentoo%20Linux) bugtracker.
2. Choose either 'Current Packages' or 'New Packages' accordingly

### Haiku Ports
Open an issue on their [Haikuports GitHub repo](https://github.com/haikuports/haikuports/issues)

### Homebrew
If you're on MacOS use: https://github.com/Homebrew/homebrew-core/blob/master/CONTRIBUTING.md

If not, then find the formula on github, edit the formula (auto-forks for you), make the appropriate changes (change the version number and get the sha256 (use another updated repo to get the the hash or download the program and run `sha256sum`), the submit a PR via github GUI.

### Hyperbola
1. Search for the package in: https://www.hyperbola.info/packages/
2. On the package page find `Flag Package Out-of-Date` link

### Linuxbrew
See Homebrew

### Macports
There are a several ways to update/request macports. Before anything, please search their github repo for [open PRs](github.com/macports/macports-ports/pulls) and their [bugtracker](https://trac.macports.org/search?q=&portsummarysearch=on) to avoid duplicate requests.
1. If you have macports installed you can go through the recommended way to update a macport
2. If you don't have macports installed you can still open a PR. You'll need to some things in the PR 
3. Open a ticket on their [bugtracker](https://trac.macports.org) requesting an update or a new package. 

### Mageia Cauldron
Open an issus on their [Bugzilla](https://bugs.mageia.org) Bugtracker

### nixpkgs
Open an issue on their [Github repo](https://github.com/NixOS/nixpkgs/)

### OpenMandriva Cooker
Open an issue on their [Bugzilla](https://issues.openmandriva.org/enter_bug.cgi?product=Cooker)

### psilinux
1. Find the package via repology or on their [GitHub organization page](https://github.com/pisilinux)  
2. Open an issue requesting update or new package.

### scoop
Open an issue on their [Github repo](https://github.com/lukesampson/scoop/issues)

### solus
Open an issue on their [Phabricator](https://dev.getsol.us/maniphest/)  
Make sure to follow their [guidelines](https://getsol.us/articles/packaging/request-a-package/en/)

### vcpkg
C++ Library Manager for Windows, Linux, and MacOS  
Open an issue on their [Github repo](https://github.com/Microsoft/vcpkg)

### Void Linux
Open an issue on their [Github repo](https://github.com/void-linux/void-packages)

### Yet Another Cygwin Ports (YACP)
Open an issue on their [Github repo](https://github.com/fd00/yacp)

#### Tips for submitting PRs
<details>
  <summary>Tips on how to submit PRs</summary>
    <ul>
      <li>Clone the repository
      <li>Edit the package forumla/recipe
      <li>Update the version number of the package
      <li>Download the updated package version
      <li>Generate a sha256 <tt>openssl dgst -sha256 package-name</tt>
      <li>Note: Macports requires a rmd160. Generate an rmd160 <tt>openssl dgst -rmd160 package-name</tt>
      <li>Submit PR
    <ul>
</details>

</details>

## FreeCAD
<table>
  <tr>
    <th>FreeCAD</th>
    <th>Dependencies</th>  
    <th>FEM Dependencies</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/freecad/versions">
        <img src="https://repology.org/badge/vertical-allrepos/freecad.svg" alt="Packaging status" align="right"></a>
    </td>
    <td align="left" valign="top">
      cmake<br/>
      python3<br/>
      qt5<br/>
      python:shiboken2<br/>
      python:pyside2<br/>
      opencascade<br/>
      opencascade-oce<br/>
      salome-smesh<br/>
      smesh<br/>
      med<br/>
      coin3d<br/>
      simage<br/>
      boost<br/>
      eigen3<br/>
      python:pivy<br/>
      xerces-c<br/>
      zlib<br/>
      graphviz<br/>
      vtk<br/>
      netgen-mesher<br/>
      python:scipy<br/>
      python:numpy<br/>
      ccache<br/>
      opencv<br/>
      gdal<br/>
      gdal-grass<br/>
      orcos-kdl<br/>
      python:matplotlib<br/>
      hdf5<br/>
      freetype<br/>
      swig<br/>
      libspnav<br/>
      spnavcfg<br/>
      zipios++<br/>
      libkdtree++<br/>
      oda-file-converter<br/>
      teighafileconverter<br/>
      luxcorerender<br/>
      luxrender<br/>
      povray<br/>
      opencamlib<br/>
      python:pycollada<br/>
      ifcopenshell<br/>
      gts<br/>
      proj<br/>
      pcl-pointclouds<br/>
      python:gitpython</br>
      expat</br>
      soqt</br>
      netcdf</br>
    </td>
    <td align="left" valign="top">
      calculix<br/>
      elmerfem<br/>
      fenics<br/>
      openfoam<br/>
      gmsh<br/>
      z88<br/>
    </td>
  </tr>
</table>

## Repology package names  
<details>
  <summary>Expand this block to view the package names in one long list</summary>

```
python3  
qt5  
python:shiboken2  
python:pyside2  
opencascade  
opencascade-oce  
salome-smesh  
smesh  
med  
coin3d  
simage  
boost  
eigen3  
python:pivy  
xerces-c  
cmake  
zlib  
graphviz  
vtk  
netgen-mesher
python:scipy  
python:numpy  
calculix  
elmerfem  
fenics  
openfoam  
z88  
gmsh  
ccache  
opencv  
gdal  
gdal-grass  
orcos-kdl  
python:matplotlib  
hdf5  
freetype
swig  
libspnav  
spnavcfg  
zipios++  
libkdtree++  
oda-file-converter  
teighafileconverter  
luxcorerender  
luxrender  
povray  
opencamlib  
python:pycollada  
ifcopenshell  
gts  
proj  
pcl-pointclouds  
python:gitpython
expat  
soqt  
netcdf  
```

</details>

## Dependencies
Below are badges generated courtesy of Repology of all 3rd party dependencies that are currently tracked via repology in the package ecosystem of Linux, MacOS, and Windows.

<table>
  <tr>
    <th>qt5</th>
    <th>python:shiboken2</th>
    <th>python:pyside2</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/qt5/versions">
      <img src="https://repology.org/badge/vertical-allrepos/qt5.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:shiboken2/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:shiboken2.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:pyside2/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:pyside2.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>opencascade</th>
    <th>opencascade-oce</th>
    <th>salome-smesh</th>
    <th>smesh</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/opencascade/versions">
      <img src="https://repology.org/badge/vertical-allrepos/opencascade.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/opencascade-oce/versions">
      <img src="https://repology.org/badge/vertical-allrepos/opencascade-oce.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/salome-smesh/versions">
      <img src="https://repology.org/badge/vertical-allrepos/salome-smesh.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/smesh/versions">
      <img src="https://repology.org/badge/vertical-allrepos/smesh.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>med</th>
    <th>python3</th>
    <th>boost</th>
    <th>netcdf</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/med/versions">
      <img src="https://repology.org/badge/vertical-allrepos/med.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python3/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python3.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/boost/versions">
      <img src="https://repology.org/badge/vertical-allrepos/boost.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/netcdf/versions">
      <img src="https://repology.org/badge/vertical-allrepos/netcdf.svg" alt="Packaging status" align="right"></a>
    </td>
</tr>
</table>

<table>
  <tr>
    <th>coin3d</th>
    <th>soqt</th>
    <th>python:pivy</th>
    <th>simage</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/coin3d/versions">
      <img src="https://repology.org/badge/vertical-allrepos/coin3d.svg" alt="Packaging status" align="right"></a>
    <td valign="top"><a href="https://repology.org/metapackage/soqt/versions">
      <img src="https://repology.org/badge/vertical-allrepos/soqt.svg" alt="Packaging status" align="right"></a>
    <td valign="top"><a href="https://repology.org/metapackage/python:pivy/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:pivy.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/simage/versions">
      <img src="https://repology.org/badge/vertical-allrepos/simage.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>hdf5</th>
    <th>eigen3</th>
    <th>xerces-c</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/hdf5/versions">
      <img src="https://repology.org/badge/vertical-allrepos/hdf5.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/eigen3/versions">
      <img src="https://repology.org/badge/vertical-allrepos/eigen3.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/xerces-c/versions">
      <img src="https://repology.org/badge/vertical-allrepos/xerces-c.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>zlib</th>
    <th>cmake</th>
    <th>ccache</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/zlib/versions">
      <img src="https://repology.org/badge/vertical-allrepos/zlib.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/cmake/versions">
      <img src="https://repology.org/badge/vertical-allrepos/cmake.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/ccache/versions">
      <img src="https://repology.org/badge/vertical-allrepos/ccache.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>netgen-mesher</th>
    <th>vtk</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/netgen-mesher/versions">
      <img src="https://repology.org/badge/vertical-allrepos/netgen-mesher.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/vtk/versions">
      <img src="https://repology.org/badge/vertical-allrepos/vtk.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>calculix</th>
    <th>gmsh</th>
  </tr>
    <td valign="top"><a href="https://repology.org/metapackage/calculix/versions">
      <img src="https://repology.org/badge/vertical-allrepos/calculix.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/gmsh/versions">
      <img src="https://repology.org/badge/vertical-allrepos/gmsh.svg" alt="Packaging status" align="right"></a>
    </td>
</table>

<table>
  <tr>
    <th>elmerfem</th>
    <th>fenics</th>
    <th>openfoam</th>
    <th>z88</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/elmerfem/versions">
      <img src="https://repology.org/badge/vertical-allrepos/elmerfem.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/fenics/versions">
      <img src="https://repology.org/badge/vertical-allrepos/fenics.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/openfoam/versions">
      <img src="https://repology.org/badge/vertical-allrepos/openfoam.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/z88/versions">
      <img src="https://repology.org/badge/vertical-allrepos/z88.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>


<table>
  <tr>
    <th>orocos-kdl</th>
    <th>python:matplotlib</th>
    <th>freetype</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/orocos-kdl/versions">
      <img src="https://repology.org/badge/vertical-allrepos/orocos-kdl.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:matplotlib/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:matplotlib.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/freetype/versions">
      <img src="https://repology.org/badge/vertical-allrepos/freetype.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>graphviz</th>
    <th>swig</th>
    <th>ifcopenshell</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/graphviz/versions">
      <img src="https://repology.org/badge/vertical-allrepos/graphviz.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/swig/versions">
      <img src="https://repology.org/badge/vertical-allrepos/swig.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/ifcopenshell/versions">
      <img src="https://repology.org/badge/vertical-allrepos/ifcopenshell.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>libspnav</th>
    <th>spnavcfg</th>
    <th>zipios++</th>
    <th>libkdtree++</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/libspnav/versions">
      <img src="https://repology.org/badge/vertical-allrepos/libspnav.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/spnavcfg/versions">
      <img src="https://repology.org/badge/vertical-allrepos/spnavcfg.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/zipios++/versions">
      <img src="https://repology.org/badge/vertical-allrepos/zipios++.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/libkdtree++/versions">
      <img src="https://repology.org/badge/vertical-allrepos/libkdtree++.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>python:scipy</th>
    <th>python:numpy</th>
    <th>opencv</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/python:scipy/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:scipy.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:numpy/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:numpy.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/opencv/versions">
      <img src="https://repology.org/badge/vertical-allrepos/opencv.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>gdal</th>
    <th>gdal-grass</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/gdal/versions">
      <img src="https://repology.org/badge/vertical-allrepos/gdal.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/gdal-grass/versions">
      <img src="https://repology.org/badge/vertical-allrepos/gdal-grass.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>oda-file-converter</th>
    <th>teighafileconverter</th>
    <th>luxcorerender</th>
    <th>luxrender</th>
    <th>povray</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/oda-file-converter/versions">
      <img src="https://repology.org/badge/vertical-allrepos/oda-file-converter.svg" alt="Packaging status" align="right"></a>
    </td>
        <td valign="top"><a href="https://repology.org/metapackage/teighafileconverter/versions">
      <img src="https://repology.org/badge/vertical-allrepos/teighafileconverter.svg" alt="Packaging status" align="right"></a>
    </td>
    </td>
        <td valign="top"><a href="https://repology.org/metapackage/luxcorerender/versions">
      <img src="https://repology.org/badge/vertical-allrepos/luxcorerender.svg" alt="Packaging status" align="right"></a>
    </td>
    </td>
        <td valign="top"><a href="https://repology.org/metapackage/luxrender/versions">
      <img src="https://repology.org/badge/vertical-allrepos/luxrender.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/povray/versions">
      <img src="https://repology.org/badge/vertical-allrepos/povray.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>opencamlib</th>
    <th>python:pycollada</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/opencamlib/versions">
      <img src="https://repology.org/badge/vertical-allrepos/opencamlib.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:pycollada/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:pycollada.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>proj</th>
    <th>gts</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/proj/versions">
      <img src="https://repology.org/badge/vertical-allrepos/proj.svg" alt="Packaging status" align="right"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/gts/versions">
      <img src="https://repology.org/badge/vertical-allrepos/gts.svg" alt="Packaging status" align="right"></a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>pcl-pointclouds</th>
    <th>python:gitpython</th>  
    <th>expat</th>
  </tr>
  <tr>
    <td valign="top"><a href="https://repology.org/metapackage/pcl-pointclouds/versions">
      <img src="https://repology.org/badge/vertical-allrepos/pcl-pointclouds.svg" alt="Packaging status"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/python:gitpython/versions">
      <img src="https://repology.org/badge/vertical-allrepos/python:gitpython.svg" alt="Packaging status"></a>
    </td>
    <td valign="top"><a href="https://repology.org/metapackage/expat/versions">
      <img src="https://repology.org/badge/vertical-allrepos/expat.svg" alt="Packaging status"></a>
    </td>
  </tr>
</table>
