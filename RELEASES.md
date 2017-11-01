# Release Notes

## [Unreleased]


## [v0.2.2] - 2017-10-26
### Added
 * New capabilities to some utility applications:
  * energymon-cmd-profile: Accept commands without quotations; add help option
  * energymon-file-provider: Add help, count, interval, and no-rewind options
  * energymon-idle-power: Add help option
 * Man pages for utility applications
 * VERSION and SOVERSION properties on shared object libraries
 * Multiarch support (use GNU standard installation directories)

### Changed
 * Increased minimum CMake version from 2.8 to 2.8.5 to support GNUInstallDirs
 * Refactor this RELEASES.md file

### Removed
 * Removed private symbol exports in shared object libraries (prevents symbol name clashes)

### Fixed
 * Various bug fixes to utility applications


## [v0.2.1] - 2017-10-01
### Added
 * Support for msr-safe kernel module in msr implementation
 * New cray-pm implementations to support capabilities of Cray XC30 and XC40 systems
 * New wattsup-libusb and wattsup-libftdi implementations
 * AppVeyor test configuration for Windows continuous integration

### Changed
 * Faster refresh in osp-polling, odroid and odroid-ioctl implementations
 * Better multi-platform support for some implementations, especially with portable time and sleep abstractions
 * Downgraded required CMake version from 2.8.9 to 2.8
 * Documented FSE 2016 and Technical Report publication information
 * Various enhancements, optimizations, and documentation improvements

### Deprecated
 * Deprecated custom DEFAULT CMake option in favor of ENERGYMON_BUILD_DEFAULT

### Removed
 * Removed Android CMake toolchain file: cmake-toolchain/android.toolchain.cmake

### Fixed
 * Fixed [#37]: In osp implementation, force overflow in ODROID Smart Power at 1000 Wh to avoid device counter saturation at 8192 Wh
 * Fixed [#27]: More modular build process
 * Numerous other bugs

## v0.2.0 - 2016-10-12
### Added
 * Initial public release

[Unreleased]: https://github.com/energymon/energymon/compare/v0.2.2...HEAD
[v0.2.2]: https://github.com/energymon/energymon/compare/v0.2.1...v0.2.2
[v0.2.1]: https://github.com/energymon/energymon/compare/v0.2.0...v0.2.1
[#37]: https://github.com/energymon/energymon/issues/37
[#27]: https://github.com/energymon/energymon/issues/27