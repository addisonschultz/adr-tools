# Help scripts

## Status

Accepted

Amends [5. Help comments](0005-help-comments.md)

## Context

Currently help text is generated by extracting specially formatted comments from the top of the command script.

This makes it easy for developers of the tool: documentation and code is all in one place.

But, it means that help text cannot include calculated values, such as the location of files.

## Decision

Where necessary, help text can be generated by a script.

The script will be called _adr\_help_\_

## Consequences

Help scripts can include helper scripts to locate files, giving more accurate instructions to the user that reflect how the tool is deployed in their environment.
