# Command Line Interface

Gauge has **first-class command line support**. If you have gauge installed, running `gauge` in terminal gives you command usage and all the flags it supports.

Here is a list of flags that can be used with `gauge`.

| Flag  | Description |Usage|
| ------| ----------- |-----|
|--add-plugin| Adds the specified non-language plugin to the current project.|```gauge --add-plugin xml-report```|
|  --api-port  |    Specifies the api port to be used.| ``` gauge --daemonize --api-port 7777```|
| --validate | Check for validation and parse errors. | ```gauge --validate specs```|
|  --daemonize    |  Run as a **daemon**.|```gauge --daemonize```|
|  --dir="."|Set the working directory for the current command, accepts a path relative to current directory.|```gauge --dir=PATH specs```|
|  --env | Specifies the **environment**. If not specified, default will be used.|```gauge --env="chrome" specs```|
|  --file, -f    | Installs the plugin from zip file. This is used with --install.|```gauge -f PATH_TO_ZIP_FILE --install java```|
|  --format      |Formats the specified spec files. |```gauge --format specs``` |
|  -g, --group   |  Specify which group of specs to execute based on -n flag.|```gauge -n=3 -g=1 specs```|
|  --init| Initializes project structure in the current directory.|```gauge --init java```|
|  --install |  Downloads and installs a plugin.|```gauge --install java```|
|  --install-all |  Installs all the plugins specified in project manifest, if not installed.|```gauge --install-all```|
|--list-templates | Lists all the Gauge templates available. | ```gauge --list-templates```|
|  --log-level |     Set level of logging to debug, info, warning, error or critical.|```gauge --log-level="debug" specs```|
|  -n          |Specify number of **parallel execution** streams.|```gauge -p -n=4 specs``` |
|  --parallel, -p |    Execute specs in parallel.|```gauge -p specs```|
|  --plugin-args | Specify additional arguments to the plugin. This is used together with --add-plugin.|```gauge --add-plugin xml-report --plugin-args="version=1.0"```|
|  --plugin-version    |         Version of plugin to be installed. This is used with --install, --uninstall, --update  .|```gauge --install java --plugin-version="0.0.5"```|
|  --refactor   |      **Refactor/Rephrase** steps.| ```gauge --refactor OLD_STEP NEW_STEP```|
|  --simple-console  | Removes colouring and simplifies the console output.|```gauge --simple-console specs```|
|  --sort, -s          |       Run specs in Alphabetical Order.|```gauge -s specs```|
| --strategy="eager" | Set the parallelization strategy for execution. Should be used with -p flag. Possible values are: eager, lazy. | ```gauge -p --strategy="lazy" specs``` |
|  --table-rows      |     Executes the specs and scenarios only for the selected rows of data table.| ```gauge --table-rows "1-3" specs/hello.spec ```|
|  --tags    | Executes the specs/ scenarios tagged with given tags. This filtering can also be done based on **tag expression**.| ```gauge --tags tag1,tag2 specs```<br>```gauge --tags "tag1 & tag2" specs```|
|  --check-updates  |Checks for Gauge and plugins updates. | ```gauge --check-updates```|
|  --update  |Updates a plugin. | ```gauge --update java```|
|  --update-all  |Updates all the installed Gauge plugins. | ```gauge --update-all```|
|  -v, --version, -version   | Print the current version and exit.| ```gauge --version```|
|  --verbose |       Enable verbose logging for debugging.|```gauge --verbose specs```|
