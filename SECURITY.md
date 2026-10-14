# Security policy

## Reporting a vulnerability

Please report privately, not in a public issue or pull request:

- Use GitHub's **Report a vulnerability** button on the Security tab of
  this repository (private vulnerability reporting):
  https://github.com/keasbeexd/blue-yeti-autoreset/security/advisories/new

Include what you found, how to reproduce it, and which commit you tested. A
proof of concept helps; please test only on your own machine.

You can expect an acknowledgement within a week. Fixes for confirmed issues
are released as soon as they are ready, with an advisory that credits you
unless you ask not to be named.

## What counts

blue-yeti-autoreset runs as root (a systemd service) and sends a reset
command to one USB device. Examples of what we want to hear about:

- a way to make it send a command to any device other than a Blue Yeti
  (`046d:0ab7`), or any command other than the volatile reset;
- anything that lets another account or a USB device make it run code,
  read or write files, or misbehave as root;
- unsafe permissions or paths in what `make install` puts in place.

This repository is a fork of Liam Rooney's original project. If a problem
is in code both share, please also tell the upstream author.

## Supported versions

Only the latest commit on the default branch is supported.
