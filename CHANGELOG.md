# Changelog
All notable changes to this project will be documented in this file.
Documented changes are those specific to Splice. 
We use `redis-by` version `3.5.3` as the base.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- We import `django` package to introduce taint-aware data types.

### Changed
- We convert `bytes` literals of `SYM_STAR`, `SYM_DOLLAR`, `SYM_CRLF`, and 
  `SYM_EMPTY` in `connection.py` to taint-aware Splice `bytes` type.