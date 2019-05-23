<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. gnat-packs - ready-build GCC/GNAT binary packages</a>
<ul>
<li><a href="#sec-1-1">1.1. x86\<sub>64</sub> Linux</a>
<ul>
<li><a href="#sec-1-1-1">1.1.1. Builds</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>

# gnat-packs - ready-build GCC/GNAT binary packages<a id="sec-1" name="sec-1"></a>

Packages are layered in order (package 2 must be installed after
package 1, package 3 after package 2)
1.  **gnat-X-base.tar.xz**
    Contains FSF GCC with C,C++, and Ada, including the full GPL
    runtime exception
2.  **gnat-X-xmlada.tar.xz**
         Contains AdaCore's xmlada library
3.  **gnat-X-gpr.tar.xz**
         Contains AdaCore's gprbuild
4.  **gnat-X-gnatcoll<sub>core</sub>.tar.xz**
         Contains AdaCore's gnatcoll-core libraries
5.  **gnat-X-src.tar.xz**
         Contains the full source collection used to build the packages

These packages are fully self-contained, and do not have any other package dependencies

Eventually, these packages will be added to appropriate package repositories.

## x86\\<sub>64</sub> Linux<a id="sec-1-1" name="sec-1-1"></a>

### Builds<a id="sec-1-1-1" name="sec-1-1-1"></a>

1.  GCC-8.3.0

    -   [gnat-8-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-base.tar.xz)
    -   [gnat-8-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-xmlada.tar.xz)
    -   [gnat-8-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-gprbuild.tar.xz)
    -   [gnat-8-gnatcoll\\<sub>core</sub>.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-gnatcoll_core.tar.xz)
    -   [gnat-8-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-src.tar.xz)

2.  Compatibility

    -   Built and tested on Ubuntu-18.04 LTS (Desktop)

3.  Installation

    1.  (For each package in order above)
        a. Verify gpg from the related signatures in this repository
           \`gpg &#x2013;verify gnat-X-y.tar.xz.sig gnat-X-y.tar.xz\`
        b. Extract the package
           \`sudo xz -cd gnat-X-y.tar.xz | tar xPf -\`
    2.  Modify ~/.bashrc or equivilent:
        -   \`export PATH=/opt/gnat-X/bin:$PATH (where X is the major version)\`
        -   \`export C<sub>INCLUDE</sub><sub>PATH</sub>=/opt/gnat-X/include\`
        -   \`export LD<sub>LIBRARY</sub><sub>PATH</sub>=/opt/gnat-X/lib64:/opt/gnat-X/lib\`
        -   \`export LIBRARY<sub>PATH</sub>=$LD<sub>LIBRARY</sub><sub>PATH\`</sub>