# dockerfile-ghe-helper

```
   ___ _ _   _        _      ___     _                    _          _  _     _               
  / __(_) |_| |_ _  _| |__  | __|_ _| |_ ___ _ _ _ __ _ _(_)______  | || |___| |_ __  ___ _ _ 
 | (_ | |  _| ' \ || | '_ \ | _|| ' \  _/ -_) '_| '_ \ '_| (_-< -_) | __ / -_) | '_ \/ -_) '_|
  \___|_|\__|_||_\_,_|_.__/ |___|_||_\__\___|_| | .__/_| |_/__|___| |_||_\___|_| .__/\___|_|  
                                                |_|                            |_|            
```

## Description

This is the Dockerfile for building Github Enterprise Helper (ghe-helper).
Github Enterprise Helper is a container platform built with tooling for
interacting with Github Enterprise and Github.com data and functionality.

## Typical Use Cases

The typical usage of this falls into the following 3 catagories.

  1. Github to Github Enterprise Migrations

  2. Github/Github Enteprise Backups

  3. Creation of markup using tooling specific for use in GH-Pages/GHE-Pages  


## References

The following resources were used in the creation of this platform.

  1. github/backup-utils
    1. https://github.com/github/backup-utils

  2. GHE
    1. https://github.com/ppouliot/ghe (Code used in this container)
    2. https://git.generalassemb.ly/ga-admin-utils/ghe (Origianl Source of the code used in this container)

