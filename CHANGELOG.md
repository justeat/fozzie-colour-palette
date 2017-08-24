# Changelog

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).


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
