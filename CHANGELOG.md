# Changelog

## [v1.3.0](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.3.0) (2024-06-06)
[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.2.0...v1.3.0)

### Added
* feat: Implement upload on public shares using dav endpoint v2 by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1225

### Changed
* refactor: Only import from nextcloud-axios not axios directly by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1224
* Updated translations
* chore(deps): Bump @nextcloud/files from 3.3.1 to 3.4.0 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1220
* chore(deps): Bump @types/node to 20.14.2 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1227

## [v1.2.0](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.2.0) (2024-05-23)
[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.1.1...v1.2.0)

### Added
* feat(NodesPicker): Add support for FileSystemEntry by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1165
* feat(ConflictPicker): Allow to use `FileSystemEntry` by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1166
* feat: Allow to upload directories and allow bulk upload by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1175
* feat: Split new-menu entries into `upload` `new` and *other* by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1206
* feat(ConflictPicker): refresh preview on etag change by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1214

### Fixed
* fix(ConflictPicker): Ensure component works also if browser does not support FileSystemEntry by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1171
* fix(ConflictPicker): Allow to set recursive upload note + fix types for conflict utils functions by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1176
* fix(docs): Add parameter docs for `getUploader` by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1207

### Changed
* Updated translations
* fix(tests): Add tests for filesystem helpers by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1174
* fix: Refactor logger and fix badges in README by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1173
* build(deps): Bump @nextcloud/dialogs to 5.3.1
* build(deps): Bump @nextcloud/auth to 2.3.0
* build(deps): Bump @nextcloud/router to 3.0.1
* build(deps): Bump @nextcloud/files to 3.2.1
* build(deps): Bump @nextcloud/l10n to 3.1.0
* build(deps): Bump @nextcloud/logger to 3.0.2
* build(deps): Bump axios to 1.7.2

## [v1.1.1](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.1.1) (2024-04-15)
[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.1.0...v1.1.1)

### :bug: Fixed bugs
* fix: Drop dependency on moment.js by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1155
* fix(upload): Do not read chunks into memory but just stream file chunks by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1153

### Changed
* Updated development dependencies
* Updated translations
* Updated @nextcloud/dialogs from 5.2.0 to 5.3.0

## [v1.1.0](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.1.0) (2024-04-02)
[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.5...v1.1.0)

### Features :rocket:
* feat: allow to specify the root of an upload by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1131
* feat: allow to specify forbidden characters by @arublov in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1132

### Bug Fixes :bug:
* fix: conflict picker by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1123
* fix: migrate conflictpicker to NcDialog and remove incorrect semantic closing icon by @emoral435 in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1113
* fix(ConflictPicker): Use action slot instead of custom wrapper for buttons by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1117

### Changed
* build(deps-dev): Bump @cypress/vue2 from 2.0.1 to 2.1.0 by @dependabot
* build(deps-dev): Bump @tsconfig/cypress from 1.0.1 to 1.0.2 by @dependabot
* build(deps-dev): Bump @types/node from 20.11.17 to 20.12.2 by @dependabot
* build(deps-dev): Bump @vitest/coverage-istanbul from 1.2.2 to 1.4.0 by @dependabot
* build(deps-dev): Bump cypress from 13.6.4 to 13.7.0 by @dependabot
* build(deps-dev): Bump typedoc from 0.25.8 to 0.25.12 by @dependabot
* build(deps-dev): Bump typescript from 5.3.3 to 5.4.3 by @dependabot
* build(deps): Bump @nextcloud/dialogs from 5.1.1 to 5.1.2 by @dependabot
* build(deps): Bump @nextcloud/files from 3.1.0 to 3.1.1 by @dependabot
* build(deps): Bump axios from 1.6.7 to 1.6.8 by @dependabot
* build(deps): Bump codecov/codecov-action from 4.0.1 to 4.1.1 by @dependabot
* build(deps): Bump dorny/paths-filter from 3.0.0 to 3.0.2 by @dependabot
* Translations updates

## New Contributors
* @emoral435 made their first contribution in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1113

## [v1.0.5](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.0.5) (2024-02-13)
[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.4...v1.0.5)

### :bug: Fixed bugs
* fix: also add `X-OC-Mtime` header to final chunks move by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1038
* fix: properly handle chunk upload failure by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1042
* fix: Add upload progress for non-chunked uploads by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1080
* fix: do not try to slice in chunk larger than the File itself by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1057
* fix: Some issues with `package.json` by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1088

### Changed
* Require NPM v10 to be compatible with LTS Node 20
* Updated translations
* Updated dependencies
* Updated development dependencies
* Migrate cypress config to use to vite by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/999
* chore: add block-unconventional-commits.yml by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1082

## [v1.0.4](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.0.4) (2023-12-15)

[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.3...v1.0.4)

### :bug: Fixed bugs
* fix(uploader): encode destination by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/996
* fix(uploader): fix PUT content-type by @skjnldsv in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1002
* fix(UploadPicker): Add label for upload progress and connect progress with description [a11y] by @susnux in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1000

### Dependencies & translations
* build(deps-dev): Bump @types/node from 20.10.3 to 20.10.4 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/990
* build(deps): Bump actions/upload-artifact from 3 to 4 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/998
* build(deps): Bump p-queue from 7.4.1 to 8.0.1 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/997
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/1003
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/993

## [v1.0.3](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.0.3) (2023-12-07)

[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.2...v1.0.3)

### :bug: Fixed bugs

* fix: do not flood with Vue errors when using in `NcBreadcrumbs` by externalizing Vue dependency [\#985](https://github.com/nextcloud-libraries/nextcloud-upload/pull/985) ([ShGKme](https://github.com/ShGKme))

## [v1.0.2](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.0.2) (2023-11-29)

## What's Changed
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/961
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/962
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/963
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/964
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/965
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/966
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/967
* enable dependabot by @szaimen in https://github.com/nextcloud-libraries/nextcloud-upload/pull/969
* build(deps-dev): Bump @types/node from 20.9.0 to 20.10.0 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/972
* build(deps-dev): Bump typedoc from 0.25.3 to 0.25.4 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/978
* build(deps): Bump @nextcloud/dialogs from 5.0.0-beta.6 to 5.0.3 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/976
* Updates for project Nextcloud upload library by @transifex-integration in https://github.com/nextcloud-libraries/nextcloud-upload/pull/968
* build(deps): Bump peter-evans/create-or-update-comment from 3.0.2 to 3.1.0 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/970
* build(deps): Bump cypress-io/github-action from 5.8.3 to 6.6.0 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/971
* build(deps): Bump actions/checkout from 3 to 4 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/974
* build(deps): Bump actions/setup-node from 3 to 4 by @dependabot in https://github.com/nextcloud-libraries/nextcloud-upload/pull/973

## New Contributors
* @szaimen made their first contribution in https://github.com/nextcloud-libraries/nextcloud-upload/pull/969

**Full Changelog**: https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.1...v1.0.2

## [v1.0.1](https://github.com/nextcloud-libraries/nextcloud-upload/tree/v1.0.1) (2023-11-17)

[Full Changelog](https://github.com/nextcloud-libraries/nextcloud-upload/compare/v1.0.0...v1.0.1)

### :bug: Fixed bugs

- fix: Do not block if the filetype is unknown to the browser [\#955](https://github.com/nextcloud-libraries/nextcloud-upload/pull/955) ([juliushaertl](https://github.com/juliushaertl))
- fix\(upload\): attach response to failed uploads too [\#953](https://github.com/nextcloud-libraries/nextcloud-upload/pull/953) ([skjnldsv](https://github.com/skjnldsv))
- Fix "Add" label to "New" [\#957](https://github.com/nextcloud-libraries/nextcloud-upload/pull/957) ([jancborchardt](https://github.com/jancborchardt))



\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*

