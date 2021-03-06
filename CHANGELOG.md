# Changelog

All notable changes to this project will be documented in this file. See [conventional-commits](https://www.conventionalcommits.org/) for commit guidelines.

## [2.1.0](https://www.github.com/terraform-google-modules/terraform-google-vm/compare/v2.0.0...v2.1.0) (2020-03-05)


### Features

* Allow the use of Google provider v3.x ([#78](https://www.github.com/terraform-google-modules/terraform-google-vm/issues/78)) ([eea5267](https://www.github.com/terraform-google-modules/terraform-google-vm/commit/eea52678b28c66d44c9cfe94a39b47fc6c496641))


### Bug Fixes

* Set target_size to null when autoscaling is enabled in MIG ([#65](https://www.github.com/terraform-google-modules/terraform-google-vm/issues/65)) ([dd71466](https://www.github.com/terraform-google-modules/terraform-google-vm/commit/dd7146642a740e779882e97725e551725ea6a04b)), closes [#64](https://www.github.com/terraform-google-modules/terraform-google-vm/issues/64)

## [2.0.0](https://www.github.com/terraform-google-modules/terraform-google-vm/compare/v1.4.1...v2.0.0) (2020-01-31)


### ⚠ BREAKING CHANGES

* Health check variables and resources were reorganized in this backwards-incompatible release. See the [upgrade guide](./docs/upgrading_to_mig_v2.0.md) for details.

### Features

* Change the readme formatting ([f2e87b3](https://www.github.com/terraform-google-modules/terraform-google-vm/commit/f2e87b3912e0095fde909cb5e0e1b4706d315edb))
* Fix healthchecks inconsistency. ([#56](https://www.github.com/terraform-google-modules/terraform-google-vm/issues/56)) ([5926dfc](https://www.github.com/terraform-google-modules/terraform-google-vm/commit/5926dfce9d38c154092132666919c539cad48f6c))

### [1.4.1](https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.4.0...v1.4.1) (2020-01-21)


### Bug Fixes

* derive project id for instance from instance template ([#63](https://github.com/terraform-google-modules/terraform-google-vm/issues/63)) ([3e2c8cd](https://github.com/terraform-google-modules/terraform-google-vm/commit/3e2c8cdeb2d0e6f1fe53bc2d0a9369c9dc59f013))

### Changed

- Replace health check related variables with a single object type parameter called `health_check` on the `mig` and
  `mig_with_percent` submodules. [#56]

## [1.4.0] - 2020-01-08

### Added

- `access_config` variable on the `umig` submodule. [#57]

### Changed

- The required Terraform provider versions are enforced. [#52]

## [1.3.0] - 2019-12-09

### Added

- Output for `tags` from `instance_template` [#33]

## [1.2.0] - 2019-11-28

### Added

- `access_config` variable on the `instance_template` and `preemptible_and_regular_instance_templates` submodules. [#43]

### Fixed

- The `region` variable is passed to all relevant resources. [#42] [#44]

## [1.1.1] - 2019-10-25
### Fixed

- Fix bug with `distribution_policy_zones` forcing permadiff. [#37]

## [1.1.0] - 2019-10-23

### Added

- Added variable `project_id`. [#26]
- `preemptible_and_regular_instance_templates` submodule. [#18]
- `mig_with_percent` submodule. [#19]
- Support for shielded VMs. [#38]

## [1.0.0] - 2019-07-31

### Added

- `preemptible` variable on the Instance Template submodule. [#14]

### Changed

- Supported version of Terraform is 0.12. [#16]

## [0.2.0] - 2019-05-30

### Added

- `instance_group` output on the `mig` submodule. [#10]

## [0.1.0] - 2019-04-30

### Added
- `instance_template`, `mig`, and `umig` modules
- examples, basic tests and fixtures for all modules

[Unreleased]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.4.0...HEAD
[1.4.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.1.1...v1.2.0
[1.1.1]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v0.2.0...v1.0.0
[0.2.0]: https://github.com/terraform-google-modules/terraform-google-vm/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/terraform-google-modules/terraform-google-vm/releases/tag/v0.1.0
[#10]: https://github.com/terraform-google-modules/terraform-google-vm/pull/10
[#14]: https://github.com/terraform-google-modules/terraform-google-vm/pull/14
[#16]: https://github.com/terraform-google-modules/terraform-google-vm/pull/16
[#18]: https://github.com/terraform-google-modules/terraform-google-vm/pull/18
[#19]: https://github.com/terraform-google-modules/terraform-google-vm/pull/19
[#26]: https://github.com/terraform-google-modules/terraform-google-vm/pull/26
[#37]: https://github.com/terraform-google-modules/terraform-google-vm/pull/37
[#38]: https://github.com/terraform-google-modules/terraform-google-vm/pull/38
[#42]: https://github.com/terraform-google-modules/terraform-google-vm/pull/42
[#43]: https://github.com/terraform-google-modules/terraform-google-vm/pull/43
[#44]: https://github.com/terraform-google-modules/terraform-google-vm/pull/44
[#52]: https://github.com/terraform-google-modules/terraform-google-vm/pull/52
[#56]: https://github.com/terraform-google-modules/terraform-google-vm/pull/56
[#57]: https://github.com/terraform-google-modules/terraform-google-vm/pull/57
