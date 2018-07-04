CHANGELOG
=========

### 1.6 - *7/4/2018*
- Added support for getting all in the `execution-queue`. Sorted by date created descending and limited to 100 results.

### 1.5 - *3/27/2018*
- Fixed bug sending the incorrect user-agent. Was previously sending the curl flag `--location` as the user-agent.

### 1.4 - *3/1/2018*
- Error exit code changed from `1` to `4` since codes 1-3 are reserved.
- `help` command now returns a successful `0` exit code instead of error.
- Added flag to curl `--location` to follow redirects.
- User-agent string passed to curl no longer sends `$USER`.
- Changes to `README.md`.
- Updated copyright to 2018. Happy New Year!
 
### 1.31 - *1/15/2017*
- Changes to `README.md`.
- Updated copyright to 2017. Happy New Year!

### 1.3 - *10/6/2016*
- Added the ability to provide a custom api endpoint by setting the environment variable `API_ENDPOINT`.

Example:

````shell
API_ENDPOINT=api.foobar.com commando servers
````

### 1.2 - *4/7/2016*
- Shellcheck and best practice cleanup.

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
