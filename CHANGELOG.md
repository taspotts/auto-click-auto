# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

- Add tests for QA

## [0.1.0-alpha.5] - 2023-08-02

### Added

- The fish configuration file for custom completions, ~/.config/fish/completions/{program_name}.fish
(notice it's specific to the program name), is created if it doesn't already exist. ~/.bashrc and
~/.zshrc configuration files, which are used to set up shell completion, are generic and we can assume
the users have already created them.

## [0.1.0-alpha.4] - 2023-07-26

### Fixed

- Handle exception when `auto-click-auto` cannot infer the shell type from the `SHELL` environment variable

## [0.1.0-alpha.3] - 2023-07-17

### Added

- Package typing information

## [0.1.0-alpha.2] - 2023-07-17

### Changed

- Function `enable_click_shell_completion` now has the `shells` positional argument set by default to `None`

## [0.1.0-alpha.1] - 2023-07-17

### Added

- Function `enable_click_shell_completion` to automatically add autocomplete support
for the Bash, Zsh, and Fish shells
- Decorator `enable_click_shell_completion_option` to easily add an option to Click commands for autocomplete
support