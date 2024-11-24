# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [0.0.2]

### Changed
- `SupportsRound` now has its outputs parameterized.
- Updated `SupportsMathFunctions` to reflect the changes to `SupportsRound`.

### Fixed
- `SupportsRound`, which was formally of the form `(int | None = None) -> Integral`, now correctly supports both options (`()` and `(int)`), similar to that of the `builtins.round` function. The new form is `() -> _T_co, (int) -> _T2_co`.
- Removed `u` from `__all__` in the main package.
