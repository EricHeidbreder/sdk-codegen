# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [21.4.0](https://www.github.com/looker-open-source/sdk-codegen/compare/looker_sdk-v21.0.0...looker_sdk-v21.4.0) (2021-04-02)


### ⚠ BREAKING CHANGES

* sdk.login, sdk.logout, and sdk.login_user will now behave exactly as the Looker API spec describes. The previous behavior can still be accessed via sdk.auth.login, sdk.auth.logout, and sdk.auth.login_user

### Features

* Looker 21.4 bindings ([#529](https://www.github.com/looker-open-source/sdk-codegen/issues/529)) ([4ecaec9](https://www.github.com/looker-open-source/sdk-codegen/commit/4ecaec93d991b9d82fd3a9ce584ee6ae8810341f))


### Bug Fixes

* auth_session uses transport_options ([#550](https://www.github.com/looker-open-source/sdk-codegen/issues/550)) ([94d6047](https://www.github.com/looker-open-source/sdk-codegen/commit/94d6047a0d52912ac082eb91616c1e7c379ab262))
* python sdk login, login_user, logout methods ([#545](https://www.github.com/looker-open-source/sdk-codegen/issues/545)) ([e55086c](https://www.github.com/looker-open-source/sdk-codegen/commit/e55086c81401092e8dbd93e273ba101e2e3efe95))

## [21.0.0]

### Added

- Looker 21.0 bindings


## [7.20.0]

### Added

- Looker 7.20 bindings - note that this package version will now follow Looker major/minor versioning.

### Fixed

- Pinning cattrs 1.1.2 for pyton >= 3.7 as 1.2.0 [has an unstructure bug](https://github.com/Tinche/cattrs/issues/119)


## [0.1.3b21]

### Fixed

- [Pass headers per sdk call](https://github.com/looker-open-source/sdk-codegen/issues/387)


## [0.1.3b20]

### Added

- Python 3.9 support

### Fixed

- cattrs and attrs version [pinning per python version](https://github.com/looker-open-source/sdk-codegen/pull/374)


## [0.1.3b19]

### Added

- [Looker 7.18 bindings](https://github.com/looker-open-source/sdk-codegen/pull/350)


## [0.1.3b18]

### Added

- [Looker 7.16 bindings](https://github.com/looker-open-source/sdk-codegen/pull/348)


## [0.1.3b17]

### Fixed

- Properties that should have been typed `Sequence[SomeEnum]` were incorrectly typed `SomeEnum` [Bug report](https://github.com/looker-open-source/sdk-codegen/issues/334) and [fix](https://github.com/looker-open-source/sdk-codegen/pull/335)


## [0.1.3b16]

### Added

- [Dictionary input/ouput support](https://github.com/looker-open-source/sdk-codegen/commit/ada7ec0f9aa122eebe391f79507b9bbe118e3882)
- [Looker 7.14 bindings](https://github.com/looker-open-source/sdk-codegen/commit/62cc1b1ceba95fe28541343bb27cd2e019ae4e35)

### Changed

- Enum generated for parameter, property, or type with an `x-looker-values` or `enum` value list declaration [#241](https://github.com/looker-open-source/sdk-codegen/pull/241), [#242](https://github.com/looker-open-source/sdk-codegen/pull/242) and [#282](https://github.com/looker-open-source/sdk-codegen/pull/282)

### Fixed

- [Use base64 encoding for OAuth session PKCE](https://github.com/looker-open-source/sdk-codegen/commit/637a0d66a352d86c236c6dea2fdd65d10fe90dd0)
