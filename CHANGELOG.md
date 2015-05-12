CHANGELOG
=========

### 1.1 - *5/12/2015*
- Added the `--silent` flag to curl to prevent progress output.

### 1.0 - *5/10/2015*
- Stable release.

### 0.7 - *5/7/2015*
- Changes to `README.md`.

### 0.6 - *5/7/2015*
- Fixed bug with command `unauth` on Linux versions of sed.

### 0.5 - *5/7/2015*
- Finished `execute` command.
- Created a curl wrapper function `curl_request`.

### 0.4 - *5/4/2015*
- Handle the case where `~/.netrc` does not exist.
- Set permissions of `~/.netrc` to `600` when running the `auth` command.

### 0.3 - *5/4/2015*
- Added `-X POST` to the curl request for command `execute`.

### 0.2 - *5/3/2015*
- Added the following new commands `execution-queue`, `executions`, `version`.
- Get the version via flags `--version` or `-v`.
- Refactoring.

### 0.1 - *5/3/2015*
- Initial development version.
