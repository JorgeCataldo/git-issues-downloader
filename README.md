# Git(hub) Issues Downloader

[![Build Status](https://travis-ci.org/remoteorigin/git-issues-downloader.svg?branch=master)](https://travis-ci.org/remoteorigin/git-issues-downloader)
[![codecov](https://codecov.io/gh/remoteorigin/git-issues-downloader/branch/master/graph/badge.svg)](https://codecov.io/gh/remoteorigin/git-issues-downloader)
[![npm version](https://badge.fury.io/js/git-issues-downloader.svg)](https://badge.fury.io/js/git-issues-downloader)

Command line application allowing you to download all issues in the CSV format from a public or private repository

## Requirements

- [Node.js](https://nodejs.org) `v10.15.0 LTS` (tested on versions `6`, `7`, `8` and `latest`)

## Installation

    npm install -g https://github.com/mkobar/git-issues-downloader

## Usage

```
Usage: git-issues-downloader [options] <repository URL>
Type git-issues-downloader --help to see a list of all options.

Options:
  -h, --help      Show help                                            [boolean]
  -v, --version   Show version number                                  [boolean]
  -u, --username  Your GitHub username - required
  -p, --password  Your GitHub password - use "none" if public repo
  -f, --filename  Name of the output file            [default: "all_issues.csv"]
  -n, --nobody    Do not display/add body             [boolean] [default: false]
  -t, --toscreen  Display to screen                   [boolean] [default: false]
```

### Examples

Command prompt will ask for username and password credentials for GitHub

```
    git-issues-downloader https://github.com/remoteorigin/git-issues-downloader
```

Example with username and password

```
    git-issues-downloader -u <username> -p <username> https://github.com/remoteorigin/git-issues-downloader
```

Use none for both if public repository

```
    git-issues-downloader -u none -p none https://github.com/remoteorigin/git-issues-downloader
```


## Development

### Project Setup

```
    git clone git@github.com:remoteorigin/git-issues-downloader.git
    cd git-issues-downloader
    npm install
```

### Run Project

```
    npm start
```

### Tests

All tests are are written in [Mocha](https://mochajs.org/) and stored in the `test` folder.

```
    npm run test
```

### Linting

Using [Standard](https://github.com/feross/standard) JavaScript linter & automatic code fixer.

```
    npm run lint
```

Automatically fix linting issues

```
   npm run lint:fix
```

## Original Code
The original github repo can be found here: 

https://github.com/remoteorigin/git-issues-downloader

Note: develop branch contains bug fixes for 0.1.3

