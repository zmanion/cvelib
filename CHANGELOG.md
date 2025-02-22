# Changelog

## [1.0.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.7.0...1.0.0) (Oct 3, 2022)

* Added support for CVE Services 2.1:
  * New subcommands: `publish`, `reject`, `undo-reject`.
  * The `show` subcommand now indluced a `--show-record` option to view a CVE's record.
  * Added several new methods in the `CveApi` interface to reflect new CVE Services API endpoints.
* Fixed sorting by the reserved timestamp when using the `list` subcommand.

## [0.7.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.6.0...0.7.0) (Feb 6, 2022)

* Reverted commit c1f5edeb2cb1a39dfbab1813a3bc68ae4c04661d, which is (for
  now) incompatible with the currently available version of CVE Services.

## [0.6.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.5.0...0.6.0) (Dec 17, 2021)

* Added prompt for API key if not specified via env var or option (#13).
* Updated list of environments to include "test".
* Renamed `reset_token` subcommand to `reset_key`.

## [0.5.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.4.0...0.5.0) (Oct 25, 2021)

* Fixed API key not being returned when creating a new user (#8).

## [0.4.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.3.0...0.4.0) (Jun 15, 2021)

* Added `cve org` command.
* Added `cve user` command.
* Refactored `Idr` interface into a general `CveApi` interface.
* Fixed error when showing a CVE that is owned by a different CNA.

## [0.3.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.2.0...0.3.0) (Jan 18, 2021)

* Fixed incorrect parsing of timestamps when using Python 3.6 (#1).

## [0.2.0](https://github.com/RedHatProductSecurity/cvelib/compare/0.1.0...0.2.0) (Jan 14, 2021)

* Fixed missing org query parameter when reserving a CVE ID.
* Improved printing of reserved CVE IDs after they are reserved.
* Improved `quota` subcommand documentation and output.

## [0.1.0](https://github.com/RedHatProductSecurity/cvelib/tree/0.1.0) (Dec 23, 2020)

* Initial public release.
