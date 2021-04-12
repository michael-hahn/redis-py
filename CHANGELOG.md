# Changelog
All notable changes to this project will be documented in this file.
Documented changes are those specific to Splice. 
We use `redis-by` version `3.5.3` as the base.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Changed
- `zset_score_pairs()` in `redis/client.py` is modified to avoid
  casting because we would lose taints.