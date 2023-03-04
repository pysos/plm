<p align="center">
  <a href="https://github.com/pysos/plm"><img alt="plm" src="https://raw.githubusercontent.com/pysos/plm/main/logo/logo.svg" width="60%"></a>
  <p align="center">The Python license manager.</p>
</p>

[![PyPi Version](https://img.shields.io/pypi/v/python-license-manager.svg?style=flat-square)](https://pypi.org/project/python-license-manager/)

<!-- [![PyPI pyversions](https://img.shields.io/pypi/pyversions/python-license-manager.svg?style=flat-square)](https://pypi.org/project/python-license-manager/) -->

PLM is a command-line tool and library that manages your Python software
licenses. Install with

```
pip install python-license-manager
```

and install a new license with

<!--pytest.mark.skip-->

```sh
plm add <your-license-key>
```

All command line options are retrieved with

<!--pytest.mark.skipif(sys.version_info < (3, 11), reason="-h output changes slightly")-->

```sh
plm -h
```

<!--pytest-codeblocks: expected-output-->

```
Usage: plm [-h] [--version]
           {list,ls,fingerprint,fp,info,i,add,a,remove,rm,clean,clear-cache,cc}
           ...

Python license manager.

Options:
  -h, --help            show this help message and exit
  --version, -v         display version information

Subcommands:
  {list,ls,fingerprint,fp,info,i,add,a,remove,rm,clean,clear-cache,cc}
    list (ls)           List all installed licenses
    fingerprint (fp)    Display machine fingerprint
    info (i)            Show license info
    add (a)             Add license
    remove (rm)         Remove license
    clean               Remove invalid licenses
    clear-cache (cc)    Clear caches
```
