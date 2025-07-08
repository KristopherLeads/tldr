# dnf download

> Download binary or source packages.
> Not default to `dnf` but supported via `dnf-plugins-core`.
> See also: `dnf`.
> More information: <https://dnf-plugins-core.readthedocs.io/en/latest/changelog.html>.

- Download the latest package to the current directory:

`dnf download {{package}}`

- Limit your package query to specific architectures:

`dnf download {{package}} --arch <{{arch1}}>[,<{{arch2}}>...]`

- Download the source `rpm` for a package:

`dnf download {{package}} --source`

- Download the `debuginfo` `rpm` for a given package:

`dnf download {{package}} --debuginfo`

- Download a package to a specific directory.

`dnf download {{package}} --downloaddir {{path/to/directory}}`

- Print a list of `URLs` where the `rpm`s can be downloaded:

`dnf download --url {{package}}`

- Limit the protocol output for the URLs printed by option `--url`:
- 
`dnf download --url --urlprotocol {{http|https|rsync|ftp}} {{package}}`

- Download all missing dependencies for the specified package:

`dnf download {{package}} --resolve`

- Download all dependencies (including already installed) for the specified package:

`dnf download {{package}} --resolve --alldeps`
