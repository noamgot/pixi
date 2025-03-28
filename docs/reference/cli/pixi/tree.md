<!--- This file is autogenerated. Do not edit manually! -->
# <code>[pixi](../pixi.md) tree</code>

## About
Show a tree of workspace dependencies

--8<-- "docs/reference/cli/pixi/tree_extender.md:description"

## Usage
```
pixi tree [OPTIONS] [REGEX]
```

## Arguments
- <a id="arg-<REGEX>" href="#arg-<REGEX>">`<REGEX>`</a>
:  List only packages matching a regular expression

## Options
- <a id="arg---auth-file" href="#arg---auth-file">`--auth-file <AUTH_FILE>`</a>
:  Path to the file containing the authentication token
- <a id="arg---concurrent-downloads" href="#arg---concurrent-downloads">`--concurrent-downloads <CONCURRENT_DOWNLOADS>`</a>
:  Max concurrent network requests, default is `50`
- <a id="arg---concurrent-solves" href="#arg---concurrent-solves">`--concurrent-solves <CONCURRENT_SOLVES>`</a>
:  Max concurrent solves, default is the number of CPUs
- <a id="arg---environment" href="#arg---environment">`--environment (-e) <ENVIRONMENT>`</a>
:  The environment to list packages for. Defaults to the default environment
- <a id="arg---frozen" href="#arg---frozen">`--frozen`</a>
:  Install the environment as defined in the lockfile, doesn't update lockfile if it isn't up-to-date with the manifest file
<br>**env**: `PIXI_FROZEN`
- <a id="arg---invert" href="#arg---invert">`--invert (-i)`</a>
:  Invert tree and show what depends on given package in the regex argument
- <a id="arg---locked" href="#arg---locked">`--locked`</a>
:  Check if lockfile is up-to-date before installing the environment, aborts when lockfile isn't up-to-date with the manifest file
<br>**env**: `PIXI_LOCKED`
- <a id="arg---no-install" href="#arg---no-install">`--no-install`</a>
:  Don't modify the environment, only modify the lock-file
- <a id="arg---no-lockfile-update" href="#arg---no-lockfile-update">`--no-lockfile-update`</a>
:  Don't update lockfile, implies the no-install as well
- <a id="arg---platform" href="#arg---platform">`--platform (-p) <PLATFORM>`</a>
:  The platform to list packages for. Defaults to the current platform
- <a id="arg---pypi-keyring-provider" href="#arg---pypi-keyring-provider">`--pypi-keyring-provider <PYPI_KEYRING_PROVIDER>`</a>
:  Specifies whether to use the keyring to look up credentials for PyPI
<br>**options**: `disabled`, `subprocess`
- <a id="arg---revalidate" href="#arg---revalidate">`--revalidate`</a>
:  Run the complete environment validation. This will reinstall a broken environment
- <a id="arg---tls-no-verify" href="#arg---tls-no-verify">`--tls-no-verify`</a>
:  Do not verify the TLS certificate of the server

## Global Options
- <a id="arg---manifest-path" href="#arg---manifest-path">`--manifest-path <MANIFEST_PATH>`</a>
:  The path to `pixi.toml`, `pyproject.toml`, or the workspace directory

## Description
Show a tree of workspace dependencies

Dependency names highlighted in green are directly specified in the manifest. Yellow version numbers are conda packages, PyPI version numbers are blue.


--8<-- "docs/reference/cli/pixi/tree_extender.md:example"
