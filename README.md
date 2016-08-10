# cite-archive-manager

Manage a CITE archive using predefined tasks in a gradle build system.

The current documentation on this page covers managing a CTS archive.


## Summary

1. Make a copy of `conf.gradle-template` as `conf.gradle`.
2. Fill out appropriate values for any CITE archives you want to work with.  (See details [below](#the-configuration-file).)
3. Run one of the gradle tasks listed below to format your repository. (See details [below](#gradle-tasks).)

## The configuration file

To configure a CTS archive, supply values for the following three settings:

1. `ctsinventory` This should be the full or relative path to a valid CTS TextInventory file.
2. `ctscitationconfig` This should be the full or relative path to a valid CTS CitationConfiguration file.
3. `ctsarchive` = This should be the full or relative path to the root
directory where editions are found. (Values for local file names in the CtsCitationConfiguration are relative to this value.)


## Gradle tasks

For working with a CTS archive:

- `gradle ctstab` Creates a tabular representation of all files in the configured archive.
