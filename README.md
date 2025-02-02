About r-ff-feedstock
====================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-ff-feedstock/blob/main/LICENSE.txt)


About r-ff
----------

Home: http://ff.r-forge.r-project.org/

Package license: GPL-2.0-or-later

Summary: The ff package provides data structures that are stored on disk but behave (almost)
as if they were in RAM by transparently  mapping only a section (pagesize) in main
memory - the effective  virtual memory consumption per ff object. ff supports R''s
standard  atomic data types ''double'', ''logical'', ''raw'' and ''integer'' and  non-standard
atomic types boolean (1 bit), quad (2 bit unsigned),  nibble (4 bit unsigned), byte
(1 byte signed with NAs), ubyte (1 byte  unsigned), short (2 byte signed with NAs),
ushort (2 byte unsigned),  single (4 byte float with NAs). For example ''quad''
allows efficient  storage of genomic data as an ''A'',''T'',''G'',''C'' factor.
The unsigned  types support ''circular'' arithmetic. There is also support for  close-to-atomic
types ''factor'', ''ordered'', ''POSIXct'', ''Date'' and  custom close-to-atomic
types.  ff not only has native C-support for vectors, matrices and arrays  with
flexible dimorder (major column-order, major row-order and  generalizations for
arrays). There is also a ffdf class not unlike  data.frames and import/export filters
for csv files. ff objects store raw data in binary flat files in native encoding,
and complement this with metadata stored in R as physical and virtual attributes.
ff objects have well-defined hybrid copying semantics,  which gives rise to certain
performance improvements through  virtualization. ff objects can be stored and reopened
across R  sessions. ff files can be shared by multiple ff R objects  (using different
data en/de-coding schemes) in the same process  or from multiple R processes to
exploit parallelism. A wide choice of  finalizer options allows to work with ''permanent''
files as well as  creating/removing ''temporary'' ff files completely transparent
to the  user. On certain OS/Filesystem combinations, creating the ff files works
without notable delay thanks to using sparse file allocation. Several access optimization
techniques such as Hybrid Index  Preprocessing and Virtualization are implemented
to achieve good  performance even with large datasets, for example virtual matrix  transpose
without touching a single byte on disk. Further, to reduce  disk I/O, ''logicals''
and non-standard data types get stored native and  compact on binary flat files
i.e. logicals take up exactly 2 bits to  represent TRUE, FALSE and NA.  Beyond basic
access functions, the ff package also provides  compatibility functions that facilitate
writing code for ff and ram  objects and support for batch processing on ff objects
(e.g. as.ram,  as.ff, ffapply). ff interfaces closely with functionality from package  ''bit'':
chunked looping, fast bit operations and coercions between  different objects that
can store subscript information (''bit'',  ''bitwhich'', ff ''boolean'', ri range
index, hi hybrid index). This allows to work interactively with selections of large
datasets and quickly  modify selection criteria.  Further high-performance enhancements
can be made available upon request.


About r-ff
----------

Home: http://ff.r-forge.r-project.org/

Package license: GPL-2.0-or-later

Summary: The ff package provides data structures that are stored on disk but behave (almost)
as if they were in RAM by transparently  mapping only a section (pagesize) in main
memory - the effective  virtual memory consumption per ff object. ff supports R''s
standard  atomic data types ''double'', ''logical'', ''raw'' and ''integer'' and  non-standard
atomic types boolean (1 bit), quad (2 bit unsigned),  nibble (4 bit unsigned), byte
(1 byte signed with NAs), ubyte (1 byte  unsigned), short (2 byte signed with NAs),
ushort (2 byte unsigned),  single (4 byte float with NAs). For example ''quad''
allows efficient  storage of genomic data as an ''A'',''T'',''G'',''C'' factor.
The unsigned  types support ''circular'' arithmetic. There is also support for  close-to-atomic
types ''factor'', ''ordered'', ''POSIXct'', ''Date'' and  custom close-to-atomic
types.  ff not only has native C-support for vectors, matrices and arrays  with
flexible dimorder (major column-order, major row-order and  generalizations for
arrays). There is also a ffdf class not unlike  data.frames and import/export filters
for csv files. ff objects store raw data in binary flat files in native encoding,
and complement this with metadata stored in R as physical and virtual attributes.
ff objects have well-defined hybrid copying semantics,  which gives rise to certain
performance improvements through  virtualization. ff objects can be stored and reopened
across R  sessions. ff files can be shared by multiple ff R objects  (using different
data en/de-coding schemes) in the same process  or from multiple R processes to
exploit parallelism. A wide choice of  finalizer options allows to work with ''permanent''
files as well as  creating/removing ''temporary'' ff files completely transparent
to the  user. On certain OS/Filesystem combinations, creating the ff files works
without notable delay thanks to using sparse file allocation. Several access optimization
techniques such as Hybrid Index  Preprocessing and Virtualization are implemented
to achieve good  performance even with large datasets, for example virtual matrix  transpose
without touching a single byte on disk. Further, to reduce  disk I/O, ''logicals''
and non-standard data types get stored native and  compact on binary flat files
i.e. logicals take up exactly 2 bits to  represent TRUE, FALSE and NA.  Beyond basic
access functions, the ff package also provides  compatibility functions that facilitate
writing code for ff and ram  objects and support for batch processing on ff objects
(e.g. as.ram,  as.ff, ffapply). ff interfaces closely with functionality from package  ''bit'':
chunked looping, fast bit operations and coercions between  different objects that
can store subscript information (''bit'',  ''bitwhich'', ff ''boolean'', ri range
index, hi hybrid index). This allows to work interactively with selections of large
datasets and quickly  modify selection criteria.  Further high-performance enhancements
can be made available upon request.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.3</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=win&configuration=win%20win_64_r_base4.3" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.4</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=1131&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-ff-feedstock?branchName=main&jobName=win&configuration=win%20win_64_r_base4.4" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--ff-green.svg)](https://anaconda.org/conda-forge/r-ff) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-ff.svg)](https://anaconda.org/conda-forge/r-ff) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-ff.svg)](https://anaconda.org/conda-forge/r-ff) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-ff.svg)](https://anaconda.org/conda-forge/r-ff) |

Installing r-ff
===============

Installing `r-ff` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-ff` can be installed with `conda`:

```
conda install r-ff
```

or with `mamba`:

```
mamba install r-ff
```

It is possible to list all of the versions of `r-ff` available on your platform with `conda`:

```
conda search r-ff --channel conda-forge
```

or with `mamba`:

```
mamba search r-ff --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search r-ff --channel conda-forge

# List packages depending on `r-ff`:
mamba repoquery whoneeds r-ff --channel conda-forge

# List dependencies of `r-ff`:
mamba repoquery depends r-ff --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-ff-feedstock
=======================

If you would like to improve the r-ff recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-ff-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/orgs/conda-forge/teams/r/)

