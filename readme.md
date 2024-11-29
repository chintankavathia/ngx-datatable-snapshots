# Temporary Workaround for Storing Git LFS Playwright Snapshots for Visual Regression Tests

This repository is a temporary solution for storing Git Large File Storage (LFS) Playwright snapshots used in the visual regression testing workflow for the [Siemens ngx-datatable](https://github.com/siemens/ngx-datatable) repository.

## Background
The `ngx-datatable` repository currently cannot store Git LFS files due to limitations with Git LFS support. As a result, this repository is used to store Playwright snapshot files generated during visual regression tests until full Git LFS support is integrated into the main repository.

## Purpose
- Store Playwright snapshot files generated from visual regression tests for `ngx-datatable`.
- Provide temporary Git LFS storage for Playwright snapshots, which cannot be handled directly within the `ngx-datatable` repository at this time.

## How It Works
This repository is used by the `ngx-datatable` workflow to handle the visual regression testing process. During testing, Playwright captures snapshots of the UI, which are then stored here. These snapshots are compared in future tests to detect visual discrepancies.

### Usage in the Workflow
- The Playwright snapshots stored in this repository are used for visual regression testing of the `ngx-datatable` library.
- The snapshots are pulled into the test workflow as part of the process to compare against new test results.

## Important Notes
- This repository is **temporary** and is meant to store only Playwright snapshots for visual regression testing purposes.
- Do not add any other files unrelated to Playwright snapshots or Git LFS content.
- Follow the [Siemens ngx-datatable repository](https://github.com/siemens/ngx-datatable) for more information.

## Future Plans
- Once Git LFS support is fully enabled in the main `ngx-datatable` repository, this repository will no longer be necessary, and the workflow will be updated accordingly.

Thank you for your understanding and cooperation.

---

*If you have any questions or suggestions, feel free to open an issue or contact the project maintainers.*
