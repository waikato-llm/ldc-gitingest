# from-gitingest-pt

* domain(s): pretrain
* generates: ldc.api.pretrain.PretrainData

Turns git repositories (local dirs or remote URLs) into text to use for pretraining. Summary and directory tree get stored in the meta-data.

```
usage: from-gitingest-pt [-h] [-l {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
                         [-N LOGGER_NAME] [-i [INPUT ...]]
                         [-I [INPUT_LIST ...]] [-p [INCLUDE_PATTERN ...]]
                         [-e [EXCLUDE_PATTERN ...]]

Turns git repositories (local dirs or remote URLs) into text to use for
pretraining. Summary and directory tree get stored in the meta-data.

options:
  -h, --help            show this help message and exit
  -l {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --logging_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}
                        The logging level to use. (default: WARN)
  -N LOGGER_NAME, --logger_name LOGGER_NAME
                        The custom name to use for the logger, uses the plugin
                        name by default (default: None)
  -i [INPUT ...], --input [INPUT ...]
                        Path or URL to the git repository to read (default:
                        None)
  -I [INPUT_LIST ...], --input_list [INPUT_LIST ...]
                        Path to the text file(s) listing the git repository
                        dirs and/or remote URLs to use (default: None)
  -p [INCLUDE_PATTERN ...], --include_pattern [INCLUDE_PATTERN ...]
                        The filename pattern for including files (default: all
                        included), see:
                        https://docs.python.org/3/library/fnmatch.html
                        (default: None)
  -e [EXCLUDE_PATTERN ...], --exclude_pattern [EXCLUDE_PATTERN ...]
                        The filename pattern for excluding files (default:
                        none excluded), see:
                        https://docs.python.org/3/library/fnmatch.html
                        (default: None)
```
