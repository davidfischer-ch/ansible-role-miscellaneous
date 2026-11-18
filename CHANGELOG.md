# Changelog

## v1.1.0 (2026-11-18)

Diff: https://github.com/davidfischer-ch/ansible-role-miscellaneous/compare/v1.0.4...v1.1.0

### Minor compatibility breaks

APT sources:

* Change `apt_new_sources_files` into a list of `{srcs, dest}` entries, each rendered to its own DEB822 file

### Features

APT sources:

* Support Ubuntu 22.04 with a classic `sources.list`
* Support Ubuntu releases after 24.04 with DEB822 sources and a stub `sources.list`
* Add Raspberry Pi OS DEB822 sources for the Debian and Raspberry Pi archives

Packages:

* Install `chrony` as the NTP daemon on Debian
* Install `chrony` as the NTP daemon on Ubuntu 26.10 and later
* Adapt the system tools to Ubuntu 26.10 and later
    * Install `7zip` instead of the virtual `p7zip-full`
    * Drop `preload`, removed from the archive

## v1.0.4 (2024-11-15)

### Features

* Ubuntu 24.04 compat

### Fix and enhancements

* Syntax

## v1.0.3 (2023-05-25)

### Features

* Add `extra_apt_packages` (default value is `[]`)

### Fix and enhancements

* Mode as string

## v1.0.2 (2022-04-06)

### Fix and enhancements

* Also install apt-utils on APT powered distributions

## v1.0.1 (2020-06-08)

### Fix and enhancements

* CentOS / RedHat 8 compatibility

## v1.0.0 (2020-03-01)

* Initial release
