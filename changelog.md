# Changelog
All notable changes to the script will be documented here

## 1.3.0 - [2024-12-23]
* Added feature to set your own `date` format via `-d` argument, followed by a valid format
* Added feature to do incremential backups via the `-l` argument followed by an integer zero or greater
* Script will look for a default exclude list, which is provided within this repo that's been shamelessly copied from [Timeshift](https://github.com/linuxmint/timeshift/blob/07f5589ecd1ff07036fa4a813292a2b5f51baefd/src/Core/Main.vala#L538)
* Relatedly, the script will look for an exclude list for your dataset.  Exclude files are stored in $HOME/.config/tar/${DATASET_NAME}.exclude.  Dataset name is derived by replacing slashes in the dataset name with a dash, removing any dots or dashes in the beginning of the dataset name.  Best way to use this is to provide the absolute path for the dataset.

## 1.2.0 - [2020-06-18] 
* Added Pushbullet notifications support using the `-p` argument
* Added `-y` argument to skip warnings (which by default, require user input to continue)

## 1.1.1 - [2020-06-17] 
* A small fix to temporary file cleanup

## 1.1.0 - [2020-06-16] 
* Added `-e` argument to exclude files / folders when generating the backup file
* Added `-v` argument for verbose output

## 1.0.0 - [2020-06-15]
* Initial release
