
upload
======


**Upload a new expansion file and attach it to the specified APK.**
### Usage
```bash
google-play expansion-files upload [-h] [--log-stream STREAM] [--no-color] [--version] [-s] [-v]
    [--credentials GOOGLE_PLAY_SERVICE_ACCOUNT_CREDENTIALS]
    [--json]
    [--type EXPANSION_FILE_TYPE]
    --package-name PACKAGE_NAME
    --expansion-file EXPANSION_FILE_PATH
    --version-code APK_VERSION_CODE
```
### Required arguments for action `upload`

##### `--package-name, -p=PACKAGE_NAME`


Package name of the app in Google Play Console. For example `com.example.app`
##### `--expansion-file, -e=EXPANSION_FILE_PATH`


Path to APK expansion file
##### `--version-code, -c=APK_VERSION_CODE`


Version code of the APK file
### Optional arguments for action `upload`

##### `--type, -t=main | patch`


The file type of the expansion file configuration which is being updated. Default:&nbsp;`main`
### Optional arguments for command `google-play`

##### `--credentials=GOOGLE_PLAY_SERVICE_ACCOUNT_CREDENTIALS`


Google Play service account credentials with JSON key type to access Google Play API. If not given, the value will be checked from the environment variable `GOOGLE_PLAY_SERVICE_ACCOUNT_CREDENTIALS`. Alternatively to entering CREDENTIALS in plaintext, it may also be specified using the `@env:` prefix followed by an environment variable name, or the `@file:` prefix followed by a path to the file containing the value. Example: `@env:<variable>` uses the value in the environment variable named `<variable>`, and `@file:<file_path>` uses the value from the file at `<file_path>`.
##### `--json, -j`


Whether to show the request response in JSON format
### Common options

##### `-h, --help`


show this help message and exit
##### `--log-stream=stderr | stdout`


Log output stream. Default `stderr`
##### `--no-color`


Do not use ANSI colors to format terminal output
##### `--version`


Show tool version and exit
##### `-s, --silent`


Disable log output for commands
##### `-v, --verbose`


Enable verbose logging for commands
