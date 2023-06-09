![Go Tool][social.image]

# 🧩 Tool

Template for a typical CLI-tool written on Go.

[![Build][build.icon]][build.page]
[![Coverage][coverage.icon]][coverage.page]
[![Quality][quality.icon]][quality.page]
[![Documentation][docs.icon]][docs.page]

[![Promo][site.icon]][site.page]
[![Mirror][mirror.icon]][mirror.page]
[![Template][template.icon]][template.page]

## 🛫 Quick start

<details>
  <summary>Work with Makefile</summary>

```bash
$ make setup
$ make help

$ make find-todos
$ make test lint
$ TIMEOUT=5s make test-with-coverage
```

</details>
<details>
  <summary>Work with Taskfile</summary>

```bash
$ alias run=./Taskfile
$ run help

$ run docs
$ run docs install build start
```

</details>
<details>
  <summary>Work with Tools</summary>

```bash
$ make tools
$ source bin/activate

$ which goimports
$ make go-fmt # goimports -local $(go list -m) -w ./...
```

</details>
<details>
  <summary>Work with Docker</summary>

```bash
$ make go-1.11 # or go-1.12, etc.
/src# make go-env 2>/dev/null | grep GOVERSION
# GOVERSION:   1.11.13
/src# make test
```

</details>

## 💡 Idea

Define a powerful template that quickly creates a new Go CLI-tool.
Not only does it provide a starting point for new projects,
but it comes equipped with pre-configured ci/cd and inventory.

```bash
$ tool do action
```

## 🏆 Motivation

At [OctoLab][octolab.site], we want to start new projects faster using best practices
with a predefined structure and focusing on core ideas implementation
rather than wasting time on environment configuration and copying boilerplate code.

## 🤼‍ How to

### Build your own module

1. [Generate][action.generate] a new repository from the template.
2. Clone the repository locally.
3. Update files:
   - `docs/CNAME`, `tools/pages/*`, `tools/*.jsx?`,
   - `go.mod`, and `README.md`:
      - [ ] 🛫 Quick start
      - [ ] 💡 Idea
      - [ ] 🏆 Motivation
      - [ ] 🤼‍ How to
      - [ ] 🛬 Integration
4. Write your code and tests.
5. 🚀

### Contribute to the template

1. Read the [contribution guidelines][docs.contrib].
2. [Fork][action.fork] the repository.
3. Make your changes.
4. Send a pull request.
5. 🤗

Before you start, please make sure your changes are in demand.
The best for that is to create [a new discussion][action.discuss],
or if you find an issue, [report it][action.issue] first.

## 🎛️ Configuration

### Pre-configured

1. [GitHub Actions](https://github.com/features/actions).
2. [GitHub Pages](https://pages.github.com).
3. [Dependabot](https://github.com/dependabot).

### Included

1. [Nextra](https://nextra.site).
2. [Makefiles](https://github.com/octomation/makefiles).
3. [Taskfiles](https://github.com/octomation/taskfiles).
4. Go tools:
   - [mockgen](https://github.com/golang/mock),
   - [golangci-lint](https://github.com/kamilsk/golangci-lint),
   - [goimports](https://github.com/kamilsk/go-tools),
   - [goreleaser](https://goreleaser.com),
   - [govulncheck](https://github.com/golang/vuln).

### Optional

1. [Bitbucket](https://bitbucket.org).
2. [Codecov](https://about.codecov.io).
3. [Slack](https://github.com/marketplace/slack-github).
4. [Settings](https://github.com/apps/settings).
5. [GitHub Socialify](https://socialify.git.ci).
6. [Go Report Card](https://goreportcard.com).
7. [Shields.io](https://shields.io).

### Coming soon

1. [CodeQL](https://codeql.github.com) (code scanning).
2. [Graphite](https://graphite.dev) (git workflow).
3. [Qodana](https://qodana.cloud) (code quality).
4. [SonarCloud](https://sonarcloud.io) (code quality).
5. [Vanity URL](https://github.com/octomation/vanity) (canonical import path).
6. [Vercel](https://vercel.com) (docs preview).

### Miscellaneous

1. [Crontab.guru](https://crontab.guru).
2. [Git History](https://githistory.xyz).

## 🧩 Installation

### Homebrew

```bash
$ brew install octolab/tap/tool
```

### Binary

```bash
$ curl -fsSL https://install.octolab.org/octomation/tool | sh
# or
$ wget -qO-  https://install.octolab.org/octomation/tool | sh
```

> Don't forget about [security](https://www.idontplaydarts.com/2016/04/detecting-curl-pipe-bash-server-side/).

### Source

```bash
# use standard go tools
$ go get go.octolab.org/template/tool@latest
# or use egg tool
$ egg tools add go.octolab.org/template/tool@latest
```

> [egg][] is the `extended go get`.

### Shell completions

```bash
$ tool completion > /path/to/completions/...
# or
$ source <(tool completion)
```

## 🤲 Outputs & outcomes

<details>
  <summary>OctoLab</summary>

- https://github.com/octolab/breakit
- https://github.com/octolab/genome*
- https://github.com/octolab/parallel*
- https://github.com/octolab/testit
- https://github.com/octolab/try*

</details>
<details>
  <summary>Octomation</summary>

- https://github.com/octomation/maintainer

</details>
<details>
  <summary>Tact.app</summary>

- https://github.com/tact-app/airseat
- https://github.com/tact-app/fiddle
- https://github.com/tact-app/loop
- https://github.com/tact-app/secret

</details>
<details>
  <summary>Others</summary>

- https://github.com/kamilsk/bridge
- https://github.com/kamilsk/check*
- https://github.com/kamilsk/egg*
- https://github.com/kamilsk/forward*
- https://github.com/kamilsk/grafaman
- https://github.com/kamilsk/lift*

</details>

<p align="right">made with ❤️ for everyone by OctoLab</p>

[social.image]:      https://socialify.git.ci/octomation/go-tool/image?description=1&font=Raleway&language=1&name=1&owner=1&pattern=Circuit%20Board&theme=Light
[awesome.icon]:      https://awesome.re/mentioned-badge.svg
[awesome.page]:      https://awesome-go.com/project-layout/
[build.icon]:        https://github.com/octomation/go-tool/actions/workflows/ci.yml/badge.svg
[build.page]:        https://github.com/octomation/go-tool/actions/workflows/ci.yml
[coverage.icon]:     https://codecov.io/gh/octomation/go-tool/branch/main/graph/badge.svg
[coverage.page]:     https://codecov.io/gh/octomation/go-tool
[quality.icon]:      https://goreportcard.com/badge/go.octolab.org/template/tool
[quality.page]:      https://goreportcard.com/report/go.octolab.org/template/tool
[docs.icon]:         https://pkg.go.dev/badge/go.octolab.org/template/tool.svg
[docs.page]:         https://pkg.go.dev/go.octolab.org/template/tool
[site.icon]:         https://img.shields.io/badge/site-GitHub%20Pages-brightgreen
[site.page]:         https://go-tool.octolab.org
[mirror.icon]:       https://img.shields.io/badge/mirror-Bitbucket-blue
[mirror.page]:       https://bitbucket.org/kamilsk/go-tool
[template.icon]:     https://img.shields.io/badge/template-go--tool-blue
[template.page]:     https://github.com/octomation/go-tool

[action.discuss]:    https://github.com/octomation/go-tool/discussions/new/choose
[action.fork]:       https://github.com/octomation/go-tool/fork
[action.generate]:   https://github.com/octomation/go-tool/generate
[action.issue]:      https://github.com/octomation/go-tool/issues/new/choose
[docs.contrib]:      https://github.com/octomation/.github/blob/main/.github/CONTRIBUTING.md
[octolab.site]:      https://github.com/octolab
[wiki.compat]:       https://en.wikipedia.org/wiki/Backward_compatibility
[wiki.gomod]:        https://github.com/golang/go/wiki/Modules

[egg]:               https://github.com/kamilsk/egg
