# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.4] - 2024-08-01

### Added

- Drop Python 3.7 support.
- 'compatibility_mode' option in `API` class to to [bypass some servers' limitations processing HTTP verbs](https://developer.wordpress.org/rest-api/using-the-rest-api/global-parameters/#_method-or-x-http-method-override-header).

## [1.1.3] - 2023-11-19

### Changed

- Allow to specify a backoff time for retries with `retry_backoff`.
- Improved the documentation in the README file.

## [1.1.2] - 2023-11-18

### Fixed

- Improper handling of status code 429 (Too Many Requests).

## [1.1.1] - 2023-11-18

### Changed

- Raise `httpx.TimeoutException` instead of a generic `Exception` on max retries exceeded.

## [1.1.0] - 2023-11-17

### Added

- Support for retries on failed requests (param `max_retries`)

## [1.0.1] - 2023-11-12

### Added

- `py.typed` marker file.

## [1.0.0] - 2023-11-12

### Added

- async API based on the original code in [https://github.com/woocommerce/wc-api-python](https://github.com/woocommerce/wc-api-python).
