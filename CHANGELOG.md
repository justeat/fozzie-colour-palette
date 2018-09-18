# Changelog

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

v2.1.0
------------------------------
*Sept 19, 2018*

### Changed
- Menulog `$green--dark` updated.
- Secondary colour updated to be `$orange` for the Menulog theme.

### Removed
- More Menulog theme updates.  Removed custom Menulog `$red` overrides (as no longer required – the red and orange were very close in colour).


v2.0.0
------------------------------
*Sept 7, 2018*

### Changed
- Menulog theming updated (breaking change).
  The Menulog colours are now specified as a mixin that is called as part of individual modules if the $theme variable is set to 'ml'.  This is so that each project importing fozzie modules only has to specify the theme variable once and each module will take care of it's own colour/variable overrides.
- Menulog Colour Scheme has been updated in line with the global UI palette provided by AU design team.


v1.4.0
------------------------------
*June 20, 2018*

### Added
- Added `prepare` npm script.
- Added `lint` script to Travis config.
- Added `files` property to `package.json` so that only the relevant files are published to npm.

### Changed
- Bumped DangerJS version.
- Updated DangerJS config.
- Updated Travis config.
- Updated license date.
- Updated details in `package.json`.


v1.3.0
------------------------------
*June 20, 2018*

### Added
- Added SCSS lint script.


v1.2.1
------------------------------
*June 19, 2018*

### Fixes
- Fixes linting error introduced in 1.2.0


v1.2.0
------------------------------
*June 19, 2018*

### Added
- Added menulog styles


v1.1.0
------------------------------
*April 19, 2018*

### Changed
- Updated `$brand--red` in line with new web palette


v1.0.0
------------------------------
*April 16, 2018*

### Changed
- Brand colours (for larger text and background highlights) modified in line with UI design updates.  main changes:
  - `$green--light` has been removed and replaced by `$brand--green`
  - `$pink` has been replaced by `$brand--pink`
  - `$brand--blue`, `$brand--orange` and `$brand--red` have been updated.

### Removed
- `$brand--lime` has been removed


v0.9.2
------------------------------
*February 5, 2018*

### Fixed
- PR template image publicly available


v0.9.1
------------------------------
*January 31, 2018*

### Fixed
- `$color-bg--accept` alias is corrected.


v0.9.0
------------------------------
*October 27, 2017*

### Added
- `$color-text--success`, `$color-text--danger`, `$color-text--warning` aliases added.


v0.8.1
------------------------------
*October 24, 2017*

### Updated
- `$color-focus-outline` updated to `$orange--light`.


v0.8.0
------------------------------
*October 20, 2017*

### Added
- `$color-focus-outline` added.


v0.7.0
------------------------------
*October 18, 2017*

### Changed
- Moved `gulp-build-fozzie` into `devDependencies`.


v0.6.0
------------------------------
*August 24, 2017*

### Added
- `$color-headings--highlight` added.


v0.5.0
------------------------------
*August 21, 2017*

### Changed
- Updated `gulp-build-fozzie` version.

### Removed
- Removed config file and directory.


v0.4.0
------------------------------
*August 8, 2017*

### Fixed
- Use of `--offWhite` was inconsistent in it’s casing across variables.  Has now been normalised.
- `$green--dark` was actually an orange colour (as it was listed wrong in the design spec).

### Changed
- Updating background variable colour names to be consistent with the naming of other colour variables.
- `$hr-color` updated to correct shade of grey.
- `$color-border--interactive` added, for the borders of interactive elements (such as checkboxes)


v0.3.0
------------------------------
*August 8, 2017*

### Added
- Added `$color-headings` variable to provide an abstraction variable for styling heading colour consistently, in line with the brand guidelines.
- Added `$color-text--hint` variable to provide an abstraction variable for styling text hints in line with the brand guidelines.
- `dangerfile.js` added to check PRs for changelog entries and `package.json` versioning (if not marked as a trivial change).

### Changed
- License updated
- PR template updated to be more relevant


v0.2.0
------------------------------
*July 26, 2017*

### Changed
- Adjusting `$color-text` variable to match the brand guidelines for default text colour.


v0.1.0
------------------------------
*May 26, 2017*

### Added
- Base variables for the colour palette trimmed down and ported over from our current Just Eat colour palette.
