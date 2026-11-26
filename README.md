# vista-forge toolkit

The tools for writing and testing M code on a VistA, test-first, in one
download:

- `m` and `v`, the commands you type, with `m-ydb` and `m-iris`, the
  YottaDB and IRIS drivers `m` calls;
- the M Standard Library (MSL), the library your code calls for JSON,
  dates, strings, tests and more, and VSL, the routines the `v` commands
  run on the VistA, both as KIDS builds;
- worked examples, from a first program written test-first to an
  application shipped as a KIDS build;
- `AGENTS.md`, a page written for an AI assistant working with you.

## Download

Each release on the [Releases page](https://github.com/vista-forge/toolkit-releases/releases)
has one archive per platform and a `SHA256SUMS` file. Releases are for
Linux on Intel or AMD (`linux_amd64`) for now.

Download the newest release's `linux_amd64` archive and `SHA256SUMS` into
a new folder, then check and unpack it there:

```
sha256sum -c --ignore-missing SHA256SUMS
tar xzf vista-forge-toolkit_*_linux_amd64.tar.gz
```

With the GitHub CLI, this fetches both files:

```
gh release download --repo vista-forge/toolkit-releases --pattern '*_linux_amd64.tar.gz' --pattern SHA256SUMS
```

Put the unpacked folder on your `PATH` and read its `README.md`.

## What you need

Docker, and a VistA to work on: the download does not include one. The
start page's YottaDB route runs one in Docker from the public
`worldvista/vehu` image. The toolkit has been tested on a YottaDB VistA in
Docker only.

## Where to start

The start page, <https://vista-forge.github.io/forge-docs/start/>, walks
you from naming your VistA to installing MSL and running its tests.

## Licence and source

The programs are licensed under the GNU Affero General Public License,
version 3 or later, or a commercial licence: see [LICENSE](LICENSE) and
[NOTICE](NOTICE). Their source is available on request: open an issue.

## Questions and problems

Open an issue in this repository.
