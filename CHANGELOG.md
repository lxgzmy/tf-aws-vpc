# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.6.0] 2020-02-18
### Breaking
- `nacl_public_custom`, `nacl_private_custom` and `nacl_secure_custom` are now maps rather than lists. This resolves the issue where changing the list order required 2 terraform apply runs to complete the update. See the examples folder the map structure.

### Fixed
- Fixed NACL that denys traffic between public and secure subnets. 

## [0.5.1] 2019-09-19
### Fixed
- Fix the versions required to use this module

## [0.5.0] 2019-09-19
### Added
- Allow the `protocol` option in NACL rules to use either string or number

## [0.4.1] 2019-09-18
### Fixed
- Add routing to gateway VPC endpoints from both private and secure subnets

## [0.4.0] 2019-09-18
### Added
- Add feature to enable gateway VPC endpoints

## [0.3.0] 2019-09-12
### Added
- Add feature to enable VPC endpoints

## [0.2.0] 2019-06-12
- Add `nacl_allow_all_http` and `nacl_allow_all_https` to add http/https egress rules to all NACLs

## [0.1.0] 2019-06-09
- Initial release
